# Intro 

这里我记录了Git的学习笔记。

# 实践

1. 部分merge:这里将`develop`的`file-tobe-merged`合并到主分支上.

```bash
git switch main
git checkout develop file-tobe-merged.txt
```

2. 冲突预防:这里新建一个`main-copy`用来处理`merge`冲突,
然后将`main-copy`合并到主分支上.

```bash
git switch main
git checkout -b main-copy
git merge develop
git switch main
git merge main-copy
```


