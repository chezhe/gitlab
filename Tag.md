
#### 创建标签
```
git tag -a v1.4 -m 'my version 1.4'
```

#### 查看

```
git show
```

#### 远处推送标签

```
$ git push origin v1.5
Counting objects: 14, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (12/12), done.
Writing objects: 100% (14/14), 2.05 KiB | 0 bytes/s, done.
Total 14 (delta 3), reused 0 (delta 0)
To git@github.com:schacon/simplegit.git
 * [new tag]         v1.5 -> v1.5
 ```

 #### 一次性推送所有标签

 ```
 $ git push origin --tags
 ```

#### 检出标签
在 Git 中你并不能真的检出一个标签，因为它们并不能像分支一样来回移动。 如果你想要工作目录与仓库中特定的标签版本完全一样，可以使用 `git checkout -b [branchname] [tagname]` 在特定的标签上创建一个新分支：
```
$ git checkout -b version2 v2.0.0
Switched to a new branch 'version2'
```
当然，如果在这之后又进行了一次提交，`version2` 分支会因为改动向前移动了，那么 `version2` 分支就会和 `v2.0.0` 标签稍微有些不同，这时就应该当心了。

