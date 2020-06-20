# Docker Hub

## 目录

[注册](#jump1)

[登录和退出](#jump2)

[拉取镜像](#jump3)

[推送镜像](#jump4)

[](#jump)

[](#jump)

---	

<span id="jump1"></span>

## 注册

在 https://hub.docker.com 免费注册一个 Docker 账号

---

<span id="jump2"></span>

## 登录和退出

```shell
docker login
```

```shell
docker logout
```

---

<span id="jump3"></span>

## 拉取镜像

你可以通过 docker search 命令来查找官方仓库中的镜像，并利用 docker pull 命令来将它下载到本地

```shell
docker search ubuntu
```

使用 docker pull 将镜像下载到本地：

```shell
docker pull 镜像名
```

---

<span id="jump4"></span>

## 推送镜像

用户登录后，可以通过 docker push 命令将自己的镜像推送到 Docker Hub

以下命令中的 username 请替换为你的 Docker 账号用户名：

```shell
docker tag ubuntu:18.04 username/ubuntu:18.04
```

查看推送结果：

```shell
docker image ls
```