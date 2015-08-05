# 安装

## 前提

在安装 Wide 前需要搭建好 Go 开发环境：

1. 下载并安装 Go (>=1.2)
2. 确认环境变量 `GOPATH`，`GOROOT` 已经配置正确

## 基础安装

### 安装包

1. [下载](http://pan.baidu.com/s/1dD3XwOT) Wide 安装包
2. 解压到安装路径 {wide}，例如 /root/wide
3. 配置 {wide}/conf/wide.json（可选，默认配置应该可以工作）

### Docker

1. 获取镜像：`sudo docker pull 88250/wide:latest`
2. 运行：`sudo docker run -p 127.0.0.1:7070:7070 88250/wide:latest ./wide -docker=true -channel=ws://127.0.0.1:7070`

获取源码后，也可以自行构建 Wide 的 Docker 镜像：
`docker build -t 88250/wide:latest .`

