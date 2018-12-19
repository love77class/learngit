# learngit
学习GIT


git init //初始化仓库

2. git add (文件name) //添加文件到本地仓库

3. git commit -m "first commit" //添加文件描述信息

4. git remote add origin git@github.com:love77class/learngit.git   #关联远程库

5. git pull origin master --allow-unrelated-histories  // 把本地仓库的变化连接到远程仓库主分支    无法 pull 内容

因为他们是两个不同的项目，要把两个不同的项目合并，git需要添加一句代码，在 git pull 之后，这句代码是在git 2.9.2版本发生的，最新的版本需要添加 --allow-unrelated-histories 告诉 git 允许不相关历史合并

6. git push -u origin master //把本地仓库的文件推送到远程仓库  

要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；

关联后，使用命令git push -u origin master第一次推送master分支的所有内容；

此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；
