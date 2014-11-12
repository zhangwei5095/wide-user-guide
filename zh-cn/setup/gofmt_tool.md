# Go 格式化工具

默认是使用 `gofmt` 进行 Go 源码格式化的。如果要使用 `goimports`，需要做如下调整：

1. 安装 goimports：`go get -u github.com/bradfitz/goimports`
2. 停止运行 Wide 然后再修改 wide.json 中用户的 `GoFormat` 项为 `goimports`
3. 重新启动 Wide

