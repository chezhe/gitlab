
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