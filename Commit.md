### Clone

```
git clone https://github.com/libgit2/libgit2
```

### Commit

##### 检查当前文件状态

```
git status
```

如果`Changes not staged for commit`

```
$ git add Commit.md
```

这时候，变动会变为`staged`状态，这时候执行`git status`就会看到`Changes to be committed`。

执行`git status -s`，会得到简洁紧凑的格式：

```
MM Commit.md
```

执行`git diff`，可以查看尚未暂存（staged）的变动；
执行`git diff --staged`，可以查看暂存状态的变动，与`git diff --cached`效果一样。
按`Q`退出。

执行 `git commit` 提交：
```
$ git commit -m 'initial project version'
```

如果没有额外参数`-m`，就会进入`vi`的界面编辑commit信息

执行`git push`就会更新到远程分支。