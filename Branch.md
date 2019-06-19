```
git log --oneline --decorate --graph --all
git log --oneline --decorate
```

#### 创建分支

```
git branch new-branch
```

#### 切换

```
git checkout new-branch
```

#### 合并

先切到主分支
```
git checkout master
git merge new-branch
```

#### 删除

```
git branch -d new-branch
```

## 分支管理

查看每一个分支的最后一次提交
```
git branch -v
```

--merged 与 --no-merged 这两个有用的选项可以过滤这个列表中已经合并或尚未合并到当前分支的分支。
```
git branch --no-merged
```

#### 删除远程分支

```
$ git push origin --delete serverfix
```