按F12打开调试页面，
然后按下ctrl+shift+p，输入命令Capture full size screenshot，敲回车，浏览器会自动截取整个网页内容。

git 命令大全

1.git init
2.git add    //把文件修改添加到暂存区,后面可以加上指定文件
3.git commit -m '说明'   //把暂存区的所有内容提交到当前分支（master）
4.git remote add origin https://github.com/Ranting1992/gitLearn.git  //本地仓库与远程仓库关联
5.git push -u origin master   //推送，u参数会把本地的master分支内容推送的远程新的master分支，
							  //还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。

6.git log     //查看提交日志
7.git log --pretty=oneline   //查看提交日志（简化版）

8.git reset --hard HEAD   //回到上一个版本

9.git reset --hard 版本号   //回到指定的版本

10.git reflog   // 记录每一次的命令，可以找到未来（还原后的未来）版本号

11.git status 

12.git diff -- readme.txt(文件名)   //查看工作区和版本库里最新版本的区别

   **git checkout -- file   //可以丢弃工作区的修改，注意：要加--，不然就变成切换分支了


13.git checkout -b dev(分支名称)    //创建分支dev并切换到分支dev，可以在这个分支上做add 和commit 的操作

14.git branch   //查看当前分支

15.git checkout master  //切换到主分支

16.git merge dev   //把dev分支的工作成果合并到master分支上（用于合并指定分支到当前分支）

17.git branch -d dev   //删除指定分支dev