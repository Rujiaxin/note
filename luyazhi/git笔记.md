## git 增加要提交的目录
```
	git add html/texiao.html
```
## git 提交代码
```
	git commit -m '版本描述'
```
## git的历史记录
```
	git log
```
### 简易输出
```
	git log --pretty=oneline
```

## 退回到上个版本
```
	git reset --hard HEAD^
```
	>另一种写法
```
	git reset --hard HEAD~
```
上一个版本就是 HEAD^ ，上上一个版本就是 HEAD^^ ，当然往上 100 个版本写 100 个 ^ 比较容易数不过来，所以写成 HEAD~100。

## 回到指定的版本
```
	git reset --hard 1094a（某个版本的 commit id 是 1094adb...）
```
## 查看执行的每一条命令
```
	git reflog
```
## 撤销修改
```
	git checkout -- readme.txt
```
## 已添加 git add 但未提交 git commit 之前，取消修改
```
	git reset HEAD readme.txt
```

## 删除文件
```
	git rm test.txt
	git commit -m 'remove test.txt'
```

## 提交至 gitHub
git pull <远程主机名> <远程分支名>
```
	git push origin master
```