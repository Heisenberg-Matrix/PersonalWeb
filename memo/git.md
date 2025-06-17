

**分支相关**

* git branch：创建新分支

* git checkout：切换分支
  * git checkout -b（branch）：创建并切换到新分支

**提交相关**

* git add：暂存区

* git commit：



* git merge：合并分支

git rebase

git fetch

git reset



git clone

git pull



## 远程拉本地（覆盖）

完全丢弃本地的更改，并将远程仓库的内容强制拉取到本地，可以使用以下命令：

```
git fetch --all
git reset --hard origin/main 
```

- `git fetch --all`：从远程仓库获取最新的分支信息。
- `git reset --hard origin/main`：将本地分支强制重置为远程分支的状态，丢弃本地的所有更改。

### 删除多余文件

未被 Git 跟踪的文件（即那些不在 `.gitignore` 文件中，且从未被添加到 Git 仓库的文件）不会被 `git reset --hard` 命令影响。

- **Git 的设计理念**：Git 的设计原则是保护用户的数据，尤其是那些未被 Git 管理的文件。Git 不会随意删除这些文件，因为它们可能对用户很重要。

- **清理未跟踪文件**：

  ```bash
  git clean -fd
  ```

  - `-f`：强制执行。
  - `-d`：删除目录。



## 本地强行覆盖远程

本地分支是 `main`，强制推送到远程仓库的 `main` 分支，可以运行以下命令：

```
git push origin main --force
```







## 初始化+同步远程仓库

远程：终端SSH加白，利用ssh方式连接URL

git init

测试与github的连接：

```
ssh -T git@github.com
```

关联远程仓库：

```
git remote add origin git@github.com:yourusername/your-repo.git
```









## 命令介绍

git fetch



git rebase



git merge



