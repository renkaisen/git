# git的诞生

## 1.linux基础知识
	- 为什么要学习Linux
		+ git工具是基于Linux平台所使用的工具
	
	- 什么是Linux
		+林纳斯·本纳第克特·托瓦兹（Linus Benedict Torvalds, 1969年~ ），著名的电脑程序员、黑客。
		Linux内核的发明人及该计划的合作者。
     托瓦兹利用个人时间及器材创造出了这套当今全球最流行的操作系统（作业系统）内核之一。
	 现受聘于开放源代码开发实验室（OSDL：Open Source Development Labs, Inc），全力开发Linux内核。
        Linux是一套免费使用和自由传播的类Unix操作系统，是一个基于POSIX和UNIX的多用户、多任务、支持多线程和多CPU的操作系统。
		它能运行主要的UNIX工具软件、应用程序和网络协议。
		它支持32位和64位硬件。
	 Linux继承了Unix以网络为核心的设计思想，是一个性能稳定的多用户网络操作系统。
        Linux操作系统诞生于1991 年10 月5 日（这是第一次正式向外公布时间）。Linux存在着许多不同的Linux版本，但它们都使用了Linux内核。
        Linux可安装在各种计算机硬件设备中，比如手机、平板电脑、路由器、视频游戏控制台、台式计算机、大型机和超级计算机。
      严格来讲，Linux这个词本身只表示Linux内核，但实际上人们已经习惯了用Linux来形容整个基于Linux内核，并且使用GNU 工程各种工具和数据库的操作系统`
	 - Linus虽然创建了Linux，但Linux的壮大是靠全世界热心的志愿者参与的，这么多人在世界各地为Linux编写代码，那Linux的代码是如何管理的呢？
		+于是Linus选择了一个商业的版本控制系统BitKeeper，BitKeeper的东家BitMover公司出于人道主义精神，授权Linux社区免费使用这个版本控制系统。
		+原因是Linux社区牛人聚集，不免沾染了一些梁山好汉的江湖习气。
		开发Samba的Andrew试图破解BitKeeper的协议；
	
	- git诞生了
		-Linus花了两周时间自己用C写了一个分布式版本控制系统，这就是Git！
		一个月之内，Linux系统的源码已经由Git管理了！
		Git迅速成为最流行的分布式版本控制系统，
		尤其是2008年，GitHub网站上线了，
		它为开源项目免费提供Git存储，无数开源项目开始迁移至GitHub，包括jQuery，PHP，Ruby等等。
		
## 	2,安装git

		-Windows安装：
			+下载git客户端软件
		- Linux安装
			+CentOS发行版
		-Mac安装
			+打开Terminal直接输入git命令，会自动提示，按提示引导安装即可。
		
		-学习git知识网站
			- http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000
			- http://backlogtool.com/git-guide/cn/
			- http://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html
			- http://rogerdudler.github.io/git-guide/index.zh.html
			- https://git-scm.com/book/zh/v2
##  3,Shell 
		- 什么是shell
			+在计算机科学中，Shell俗称壳，用来区别于Kernel（核），
			用户可以利用 shell 与操作系统进行交互.	
			是指“提供使用者使用界面”的软件（命令解析器）
		
			它类似于DOS下的command和后来的cmd.exe。它接收用户命令，
			然后调用相应的应用程序。
		- 图形界面shell: 通过提供友好的可视化界面，调用相应应用程序，
		如windows系列操作系统，Linux系统上的图形化应用程序GNOME、KDE等。

		-命令行shell：通过键盘输入特定命令的方式，调用相应的应用程序，
		如windows系统的cmd.exe、Windows PowerShell，Linux系统的Bourne shell ( sh)、Bourne Again shell ( bash)等

	+ shell命令
		+  pwd (Print Working Directory) 查看当前目录
		+  cd (Change Directory) 切换目录，如 cd /etc
		+  ls (List) 查看当前目录下内容，如 ls -al,“.”(表示当前目录)和“..”(表示当前目录的父目录)。
		+  mkdir (Make Directory) 创建目录，如 mkdir blog
		+  touch 创建文件，如 touch index.html
		+  echo >>追加文件 >重新添加一行
		+  wc (Word Count) 字数信息统计，如 wc index.html
		+  cat 查看文件全部内容，如 cat index.html
		+  more less 查看文件，如more /etc/passwd、less /etc/passwd
		+  rm (remove) 删除文件，如 rm index.html、rm -rf  blog
		+  rmdir (Remove Directory) 删除文件夹，只能删除空文件夹，不常用
		+  mv (move) 移动文件或重命名，如 mv index.html ./demo/index.html
		+  cp (copy) 复制文件，cp index.html ./demo/index.html
		+  head 查看文件前几行，如 head -5 index.html
		+  tail 查看文件后几行 –n –f，如 tail index.html、tail -5 index.html 
		+  history 查看操作历史
		+  whoami 查看当前用户
	
## 4.git简单介绍
		- 什么是git
			+ git Git是一款源代码管理工具（版本控制工具）

## 5,现在常用的版本控制系统的两个模型
		svn  集中式管理
		git  分布式管理

## 6，git命令使用
		- git 初次使用添加用户名和邮箱
		+配置用户名:'git config --global user.name '您的用户名'
		+配置邮箱:'git config --global user.email '您的邮箱''
		+查看配置:'git config --list'
		
## 7,如何使用git
		--> 初始化git 仓库    
			+ `git init`
			+ 这个命令会在当前目录中新建一个隐藏的名为.git的文件夹,里面存储的是项目的各个版本
		
		-->查看当前的仓库状态 
			+ `git status`
			+ 查看当前工作目录的状态，是已经放到暂存区，还是提交到仓库了。
		
		-->把我们的代码，放到暂存区  
			+ git add 文件名/文件夹
				- 表示将文件/文件夹添加到暂存区
			+ git .  / git *
				- 表示将当前目录中所有文件添加到暂存区
			+ 可以对文件执行多次add命令，都会把最新的修改添加到暂存，但是，后页面执行add命令，
			会把前面执行add命令添加到暂存区的文件覆盖(相同的文件会覆盖)
		-->将文件添加到仓储中
			+ `git commit -m` '这次是我一个次提交的代码'
				- -m 表示需要指定一个字符串,表示本次提交代码的说明，类似于写注释 
			
		--> 查看日志
			+ 命令:` git log`
			+ 或命令:'git log --oneline'
			
		

## 	8,版本回退
		--> 命令 `git reset --hard head`
				-回到最近一次提交的版本的文件状态
				- `git reset --hard Head^^ 表示回到最近往前第二次的提交
				- Head 后面的^表示回退到第几次
		--> 命令 `git reset --hard Head~1`
				- 回到最近一次提交的前一次提交
				- Head~2 回退到最近一次提交的前2次提交
		--> 命令 `git reset --hard [版本号]`
				- 回退到某个具体的版本
				- 可以配合git reflog命令查看历史操作来进行回退 
	
## 9,创建git分支
		+ 正在做功能呢，才做了一半，但是为了不丢失代码要提交，又不能影响别人工作。
		+ 查看有多少分支
			- `git branch`
		+ 命令: git branch dev
			- 创建了一个名为dev的分支
		+ 命令: git checkout dev
			- 切换到dev分支
		+ 创建并切换到指定分支
			- `git checkout -b dev`
	- 合并Git分支
		
		+ 命令: git merge dev
			- 表示将当前分支与dev分支合并
			- 在主分支下执行合并命令. 
		+ 命令: git branch -d dev
			- 表示删除dev分支,当合并分支后，如果不需要再使用dev分支，则可以直接删除。
			- 不要在dev分支执行这个命令，在别的的分支执行.
			- 解决冲突
				+ 应该是如何合并冲突。
				+ 冲突是不可避免的。
				+ 当在新功能完成后合并前，修改并提交了主分支对应的文件，合并时两个分支中的文件有冲突。
				+ 手动修改文件，然后提交
			
## 10,git网上操作
		
		- gitHub、gitLab和国内的git网站
			+ 这些托管网站就相当于 百度云盘、360云盘 只不过这里上传的是源代码而不是其他东西
			+ gitHub大部分收费  [官网地址](https://github.com)
			+ gitLab大部分免费 [官网地址](https://gitlab.com)
	   - git clone
			 + 命令:'git clone [仓储地址]'
			 + 会把指定仓储的整个下载来
			 + 如果不需要下载整个仓储，只需要最新的一次提交,加上参数--depth
	   - 登录
			  +  直接通过账号密码登录，太麻烦了
			  +  通过SSH登录，不用在输入用户名和密码
				- 1.在任意位置输入 ssh-keygen -t rsa 创建rsa密钥
				- 2.将rsa密钥给网站
				- 3.选clone路径的时候选择ssh登录
			  + ssh的方式
				- 在本地生成一个秘钥与一个明钥,将这个公钥赋值到远程项目中,那么就可以实现‘不登录’下载了
				
				
	   - push（推送）
			  + 命令：`git push [地址] master`
			  + 或命令：`git push origin master`
	   - pull（拉回)
			  + 命令：`git pull [地址] master`
			  + 或命令：`git pull origin master`
	   - remote命令使用
			  + git remote add “主机名称” “远程仓库地址”添加远程主机，即给远程主机起个别名，方便使用
			  + git remote rm“主机名称” 命令用于删除远程主机。
			  + git remote 可以查看已添加的远程主机
			  + git remote show “主机名称”可以查看远程主机的信息
## 11,如何提交到gitHub上
		1，创建一个以自己名字.github.io 的仓储库
		2，通过git提交代码
			- git status 查看当前工作目录的状态，是已经放到暂存区，还是提交到仓库了。
			- git add . 提交到暂存区
			- git status 查看当前状态
			- git commit -m '抒写注释'  提交到仓库
			- git push github地址 master  - 提交到github
			
		创建 用户名.github.io/仓储名访问   分支连接(路由连接)
		- 同上 首先提交到master分支
			github自带的gh-pages的分支 ,创建分支并转到gh-pages分支
		- `git checkout -b gh-pages`
		- 最后把代码推到github 
		- 用户名.github.io/仓储库

		
	