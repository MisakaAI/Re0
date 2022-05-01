# 镜像

## 搜索

```bash
# docker search [关键词]
docker search centos
```

## 获取

```bash
# docker pull [选项] [Docker Registry 地址[:端口号]/]仓库名[:标签]
docker pull centos
```

## 使用

```bash
docker run -it --rm centos bash
# docker run 运行容器
# -i 交互式操作
# -t 使用终端
# --rm 退出容器后立即删除
# centos 选择容器运行使用的镜像
# bash 命令
```

## 列出

```bash
# 列出已下载的镜像
docker image ls
docker images
# 显示虚悬镜像(仓库命标签均为 <none>)
docker image ls -f dangling=true
# 删除虚悬镜像(没有价值，随意删除)
docker image prune
# 显示包括中间层镜像在内的所有镜像
docker image ls -a
```

## 删除

```bash
# docker image rm [选项] <镜像1> [<镜像2> ...]
docker image rm centos          # 镜像名
docker image rm ubuntu:19.04    # <仓库名>:<标签>
docker image rm fce289e99eb9    #完整 ID
docker image rm fce             # 短 ID (取前3个字符以上)
```

## 将容器保存为镜像(commit)

<span style="color:red;">不要使用 docker commit 定制镜像</span>
以当前的容器状态生成镜像，不会记录对原镜像所进行的操作，不便于后续维护
应使用 Dockerfile 生成镜像

```bash
# docker commit [选项] <容器ID或容器名> [<仓库名>[:<标签>]]
docker commit \
    --author "AUTHOR" \     # 修改作者
    --message "MESSAGE" \   # 修改说明
    ubuntu \                # 容器名
    ubuntu:latest           # 仓库名:标签
```
