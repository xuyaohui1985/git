
## 通过命令行创建仓库并提交到远端
```
echo "# git" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/xuyaohui1985/git.git
git push -u origin master
```

## …or push an existing repository from the command line
```
git remote add origin https://github.com/xuyaohui1985/git.git
git push -u origin master
```

#### [git远程分支创建](https://blog.csdn.net/linlin_xia/article/details/53897808)


## 添加分支

#### 分支查看
	git branch：查看本地分支 

	git branch -r：查看远程分支  

	git branch -a 查看所有分支。其中带有remote的，代表远程分支  

1. git branch `分支名称dev`
2. git checkout `分支名称dev`，切换到dev分支
   创建并切换分支：git checkout -b `分支名称`

3. git push -u origin `分支名称dev`，提交到远程服务器，并在远程服务器创建分支dev。

## 删除分支
1. 删除本地分支，git branch -d `分支名称dev`。
2. 删除远程分支，git push origin --delete `分支名称dev`。

#### 直接删除远程分支
1. 查看远程分支 git branch -a
2. 删除远程分支`dev` git branch -r -d origin/dev
3. 提交，git push origin :dev


#### 重命名文件（包括大小写）[当git上文件名大小写重命名的修改时](https://www.cnblogs.com/samwang88/p/6611947.html)

1. git mv git.md Git.md
2. commit到本地，然后push到远程仓库

