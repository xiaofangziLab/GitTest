Git help
从现在起，只要本地作了提交，就可以通过命令：
git push origin master

现在，我们根据GitHub的提示，在本地的learngit仓库下运行命令：

$ git remote add origin git@github.com:michaelliao/learngit.git

就可以把本地库的所有内容推送到远程库上：

$ git push -u origin master
=====================================================-----------
要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；

关联后，使用命令git push -u origin master第一次推送master分支的所有内容；

此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；
===============================================================