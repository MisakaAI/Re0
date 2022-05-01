# OPENSSL生成SSL自签证书

## 生成私钥

openssl genrsa -des3 -out server.key 4096
#生成rsa私钥，des3算法，4096位强度，server.key是秘钥文件名。

## 删除私钥中的密码
openssl rsa -in server.key -out server.key

## 生成CSR（证书签名请求）
openssl req -new -key server.key -out server.csr

```
Country Name (2 letter code) [AU]:国家名称（2个字母代码）
State or Province Name (full name) [Some-State]:州或省名（全称）
Locality Name (eg, city) []:Qingdao地区名称（如城市）
Organization Name (eg, company) [Internet Widgits Pty Ltd]:组织名称（例如，公司）
Organizational Unit Name (eg, section) []:组织单位名称（如，章节）
Common Name (e.g. server FQDN or YOUR name) []:域名
Email Address []:电子邮件地址

Please enter the following 'extra' attributes请输入以下“额外”属性
to be sent with your certificate request与您的证书申请一起发送
A challenge password []:提议密码
An optional company name []:可选公司名称
```

## 生成自签名证书
openssl x509 -req -days 365 -in server.csr -signkey server.key -out server.crt
