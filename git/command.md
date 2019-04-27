删除远程分支
```
	git push origin --delete xxx
```
删除本地分支
```
	git branch -d/-D  xxx
```
撤销本地修改，返回到上一次add 或者上一次 commit
```
	git checkout -- <file>
```
撤销commit
```
	git reset  <commit id>   保留修改的内容在工作区
	git reset  --hard  <commit id> 不保留修改的内容
```

拉取远程指定分支
```
    git fetch origin xxx:xxx  前一个xxx是远程分支名,后一个xxx是本地分支名
```
