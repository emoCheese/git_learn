# Git 使用教程

## git 基本命令

```bash
# 在当前目录下初始化本地仓库
git init 

# 添加文件
git add 文件
# 添加所有文件
git add .

```



```bash
# 提交
git commit -m "写提交的信息"
```

> 其中 -m 参数为简短提交的信息后面跟 "" ， 不带 -m 则会进入文本编辑器或vim写入提交信息 



```bash
# 添加远程仓库 
git remote add [别名] [仓库地址]

# 查看当前仓库所对应的远程仓库的别名和地址
git remote -v

# 从远程仓库拉取最新的提交到本地仓库
git pull 
```

### Git 分支

1. **创建分支**: 使用 `git branch [分支名]` 命令来创建一个新的分支，并指定分支名称。例如：

   ```bash
   git branch new-feature
   ```

2. **切换分支**: 使用 `git checkout [分支]` 命令来切换到指定的分支。例如：

   ```bash
   git checkout main
   ```

3. **创建并切换到新分支**: 也可以通过 `git checkout -b [分支]` 命令来一步完成创建并切换到新分支的操作。例如：

   ```bash
   git checkout -b new-feature
   ```

4. **合并分支**: 在合并分支时，通常会指定要合并的目标分支。例如，将 `feature` 分支合并到 `main` 分支：

   ```bash
   git checkout main
   git merge feature
   ```

5. **删除分支**: 要删除一个分支，可以使用 `git branch -d [分支]` 命令。例如：

   ```bash
   git branch -d old-feature
   ```

6. **查看分支列表**: 可以使用 `git branch` 命令来列出所有分支，并显示当前所在的分支。例如：

   ```bash
   git branch
   ```

这些是在 Git 中指定分支名称时常见的情况和相关操作。

