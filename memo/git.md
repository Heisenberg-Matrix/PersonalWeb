

## 远程拉本地（覆盖）

完全丢弃本地的更改，并将远程仓库的内容强制拉取到本地，可以使用以下命令：

```
git fetch --all
git reset --hard origin/main 
```

- `git fetch --all`：从远程仓库获取最新的分支信息。
- `git reset --hard origin/main`：将本地分支强制重置为远程分支的状态，丢弃本地的所有更改。



## 本地强行覆盖远程

本地分支是 `main`，强制推送到远程仓库的 `main` 分支，可以运行以下命令：

```
git push origin main --force
```

