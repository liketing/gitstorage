Git is a version control system.
Git is free software.

--安装
1、安装后设置用户名和邮件
	$ git config --global user.name "Your Name"
	$ git config --global user.email "email@example.com"

--创建版本库
1、创建版本库，即创建一个空的文件夹
2、初始化，使其变成Git仓库：git init
3、把文件添加到仓库：git add xxx.txt
4、添加后要进行提交：git commit -m "提交说明"


--时光机穿梭
1、查看现在版本库状态：git status
2、对比版本不同文件的内容：git diff xxx.txt
3、将修改后的文件先添加，再提交

--退回
1、查看提交日志：git log [--pretty=oneline]
2、回退：git reset --hard 编号
3、查看文档：cat xxx.txt
4、查看全部日志：git reflog