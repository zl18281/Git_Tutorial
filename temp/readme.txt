This is a github tutorial.

1. Install Git

	On Linux:
		sudo apt-get install git

2. 创建项目文件夹

	在系统的某个地方建立project folder

3. 初始化本地仓库

	进入projext folder， 打开terminal，输入：git init
	project folder里会生成一个隐藏文件夹.git

4. 设置username和user邮箱

	git config --global user.name "xxx"
	git config --global user.email "xxx"

5. 项目改动

	修改项目里的文件夹、文件后，输入： git status, git会显示改动还没有放入stage区域
	输入： git add . ，git会把改动放入stage区域， 再次输入git status，会显示还没有commit
	输入： git commit , git会把改动放入本地版本控制系统

6. 创建github远程仓库

	1）注册
	2）本地生成SSH key
		生成SSH Key：ssh-keygen –t rsa –C "你的邮箱@xx.com"
		生成Key时弹出选项，回车选择默认即可。
		Key保存位置：/root/.ssh
		登陆GitHub，创建new SSH key，其内容为/root/.ssh/id_rsa.pub中文本
	3）创建github repo， 复制url

7. 将本地repo push到github

	1）关联本地仓库和GitHub库：git remote add origin 网站上的仓库地址
	第一次将本地仓库推送到GitHub上：git push –u origin master

	2）本地库的改动提交到远程库：git push origin master
	更新本地库至远程库的最新改动：git pull
