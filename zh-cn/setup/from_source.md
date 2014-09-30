# 从源代码安装

## 前提

1. 搭建好 Go 开发环境
2. 安装好 git

## 步骤

1. 通过 ````git clone```` 或下载 zip 包方式获取 Wide 源码（项目地址：https://github.com/b3log/wide）
2. 获取依赖，在 Wide 源码目录下执行：
   * ````go get -u````
   * ````go get -u github.com/88250/ide_stub````
   * ````go get -u github.com/nsf/gocode````
3. 编译：在 Wide 源码目录下执行 go build
4. 配置 {wide}/conf/wide.json（可选，默认配置应该可以工作）
5. 运行可执行文件 wide 或 wide.exe

