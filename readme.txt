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

--撤销修改
1、撤销修改：git checkout --xxx.txt
	如果没有提交，则撤销到暂存区一致
	如果提交到了暂存区，则撤销和正式区一致
	如果提交到了正式区，就需要执行回退操作
	
--删除文件
1、如果你将本地的文件删除了。你可能是因为两点
	a)你确实要删除这个文件，你需要执行：git rm xxx.txt ;git commit -m "删除文件xxx.txt" 来删除版本库中的文件
	b)你删错了，你需要重新从版本库中下载一份：git checkout --xxx.txt
	
--Github远程仓库
1、注册Github账号
2、在本地仓库执行：ssh-keygen -t rsa -C "你的email地址"，创建ssh key
3、在Github远程仓库中将sshkey 配进去
4、如果有多台计算机就配置多个key

--添加远程仓库



























