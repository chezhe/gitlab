
### Log

执行`git log`会输出类似下面的信息
```
commit 02bd5e41c7c648a72da2fcdbdbd853c6444fcecc (HEAD -> master, origin/master, origin/HEAD)
Author: chezhe <chezhe17@gmail.com>
Date:   Tue Jul 10 11:13:41 2018 +0800

    branch

commit 7c1eb99223db8abe033853c8e9434197206f3543
Author: 王亮 <chezhe17@gmail.com>
Date:   Thu May 10 13:29:52 2018 +0800

    something about push

commit a919e3ce5eb078269e51394113349fdb6922539a
Author: 王亮 <chezhe17@gmail.com>
Date:   Thu May 10 13:28:35 2018 +0800
```

`git log` 有许多选项可以帮助你搜寻你所要找的提交，一个常用的选项是 -p，用来显示每次提交的内容差异。 你也可以加上 -2 来仅显示最近两次提交。

如果你想看到每次提交的简略的统计信息，你可以使用 --stat 选项：

`git log --stat`

输出信息是这样的:
```
commit 02bd5e41c7c648a72da2fcdbdbd853c6444fcecc (HEAD -> master, origin/master, origin/HEAD)
Author: chezhe <chezhe17@gmail.com>
Date:   Tue Jul 10 11:13:41 2018 +0800

    branch

 Branch.md | 0
 1 file changed, 0 insertions(+), 0 deletions(-)

commit 7c1eb99223db8abe033853c8e9434197206f3543
Author: 王亮 <chezhe17@gmail.com>
Date:   Thu May 10 13:29:52 2018 +0800

    something about push

 Commit.md | 4 +++-
```

具体参考[查看提交历史](https://git-scm.com/book/zh/v2/Git-%E5%9F%BA%E7%A1%80-%E6%9F%A5%E7%9C%8B%E6%8F%90%E4%BA%A4%E5%8E%86%E5%8F%B2)