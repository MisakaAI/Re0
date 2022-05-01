# Docker 安装

https://docs.docker.com/engine/install/
https://vuepress.mirror.docker-practice.com/install/

## 卸载旧版本

```bash
sudo apt-get remove docker docker-engine docker.io containerd runc
```

## 设置 Docker 的存储库

```bash
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg lsb-release -y
```

## 添加 Docker 的官方 GPG 密钥

```bash
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
```

## 设置稳定存储库

### 官方源

```bash
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

### 清华大学

```bash
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://mirrors.tuna.tsinghua.edu.cn/docker-ce/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
```

## 安装 Docker 引擎

```bash
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-compose-plugin -y
```

## 列出您的存储库中可用的版本

```bash
apt-cache madison docker-ce
```

## 便捷脚本

```bash
# Raspbian 必须使用脚本安装
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```

## 国内镜像加速器

- [阿里云加速器](https://cr.console.aliyun.com/cn-hangzhou/instances/mirrors)
(点击管理控制台 -> 登录账号(淘宝账号) -> 右侧镜像工具 -> 镜像加速器 -> 复制加速器地址)
- [网易云加速器](https://hub-mirror.c.163.com)
- [百度云加速器](https://mirror.baidubce.com)