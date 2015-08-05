# Docker

1. 获取镜像：`sudo docker pull 88250/wide:latest`
2. 运行：`sudo docker run -p 127.0.0.1:7070:7070 88250/wide:latest ./wide -docker=true -channel=ws://127.0.0.1:7070`

获取源码后，也可以自行构建 Wide 的 Docker 镜像：
`docker build -t 88250/wide:latest .`