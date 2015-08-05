# 常见问题与解答

* **默认用户是？**

  默认用户是 admin 用户。用户名：admin，密码：admin。

* **wide.json 是什么？**

  wide.json 是 Wide 的配置文件，路径是 {wide}/conf/wide.json。Wide 的所有配置（例如服务 IP、端口、区域等）都是保存在这个文件中的。

  如果 Wide 是个人使用，那么默认的配置应该可以很好的工作，不需要修改任何地方。

* **什么是工作空间？**

  工作空间是当前用户的 $GOPATH 路径，一个用户只能有一个工作空间。

* **Windows上构建时出现“Access is denied”**

  请“以管理员身份运行”。

* **文件树里的 Go API 目录是什么？**

  该目录是读取 $GOROOT/src 生成的，方便用户查看 Go API 源代码。 在该目录下是不允许新建、编辑、删除文件的。

* **为什么代码辅助功能（自动完成/跳转到声明等）失效了？**

  请确认正确安装了 gocode 和 gotools 工具。安装命令：
  * `go get -u github.com/visualfc/gotools`
  * `go get -u github.com/nsf/gocode`

  如果安装不正确，Wide  会自动检查并通过通知窗口告知用户。另外，通知窗口还会告知用户一些其他重要信息，例如 IDE 版本更新提醒等。

