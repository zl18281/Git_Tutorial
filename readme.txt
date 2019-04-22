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

6. xxx
