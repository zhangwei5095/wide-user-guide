# 多用户配置

## 步骤

1. 初始化主库：在 {wide}/data/workspace/src 下执行 git init
2. **添加用户：修改 {wide}/conf/wide.json 中的 Users**
3. 添加用户库：在 {wide}/data/user_workspaces/{user}/src 中 git clone 主库

Git 相关不是必须的。
