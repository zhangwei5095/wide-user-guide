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

### 自行构建

1. [下载](https://github.com/b3log/wide/archive/master.zip) 或通过 `git clone https://github.com/b3log/wide` 获取源码
2. 安装依赖：在源码目录下执行 `go get`，然后再执行 `go get github.com/visualfc/gotools github.com/nsf/gocode github.com/bradfitz/goimports`
3. 编译 Wide：`go build`

### Docker

1. 获取镜像：`sudo docker pull 88250/wide:latest`
2. 运行：`sudo docker run -p 127.0.0.1:7070:7070 88250/wide:latest ./wide -docker=true -channel=ws://127.0.0.1:7070`

获取源码后，也可以自行构建 Wide 的 Docker 镜像：
`docker build -t 88250/wide:latest .`

