# Git is a version control system.
Git is free software.

```
# 此为注释 – 将被 Git 忽略
*.a       # 忽略所有 .a 结尾的文件
!lib.a    # 但 lib.a 除外
/TODO     # 仅仅忽略项目根目录下的 TODO 文件，不包括 subdir/TODO
build/    # 忽略 build/ 目录下的所有文件
doc/*.txt # 会忽略 doc/notes.txt 但不包括 doc/server/arch.txt
```
另外 git 还提供了另一种 exclude 的方式来做同样的事情，不同的是 .gitignore 这个文件本身会提交到版本库中去。
用来保存的是公共的需要排除的文件。
而 .git/info/exclude 这里设置的 则是你自己本地需要排除的文件。 他不会影响到其他人。也不会提交到版本库中去。

> 1. 所以ignore和exclude的区别只是公共还是本地？
> 2. 根目录下，ignore和exclude都无效？


