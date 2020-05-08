# vagrant--virtualbox
用vagrant搭建virtualbox虚拟机

一、	软件安装

	VirtualBox：https://www.virtualbox.org/wiki/Downloads（Windows系统选择第一个下载）

 

	Vagrant：https://www.vagrantup.com/downloads.html（根据自己的系统配置选择下载）

 

下载完成后，点击安装，全部按照提示默认安装。安装路径可以根据自己情况更改，但要注意自己定义的安装路径不能出现中文字符。
二、	安装命令

	在非系统盘下新建一个文件夹，最好直接创建，方便寻找路径；将learn-cos-ubuntu64.box（见qq群）复制到该文件夹下

	打开命令命令提示符cmd

 

	输入 vagrant -v，若出现Vagrant的版本号，说明vagrant安装成功，方可继续往下安装

 

	进入第一步创建好的文件夹下（os就是第一步创建好的文件夹）

 

	输入：vagrant box add linux learn-cos-ubuntu64.box   回车，（其中linux是自己起的名，可随意更改）等待自动添加

	输入：vagrant init linux    回车（初始化box，其中linux是上一步中自己起的名字）

	输入：vagrant up   回车（启动虚拟机，等待自动启动，效果如下界面）

 

	此时打开安装好的virtualbox，会有如下效果，左边会多出一个正在运行的虚拟机

 

	在命令提示符输入：vagrant ssh

 

	安装完成，此时就可以在命令提示符中执行linux的一些基本命令了

说明：安装过程中若遇到任何问题，即可在群里互相讨论，共同学习

根据网上说的VirtualBox兼容性问题，在VirtualBox安装目录中找到VBoxManage.exe，右击选择属性，设置Windows Server 2008兼容模式运行。再执行vagrant up，正常运行，问题解决。





附：vagrant基本使用命令
•  vagrant box list 查看当前虚拟机
•  vagrant box add 添加一个虚拟机
•  vagrant box remove 移除虚拟机
•  vagrant init 初始化一个虚拟机
•  vagrant up 开启虚拟机
•  vagrant ssh 登录虚拟机
•  vagrant suspend 挂起虚拟机
•  vagrant reload 重启虚拟机
•  vagrant halt 关闭虚拟机
•  vagrant status查看虚拟机状态
•  vagrant destory 删除虚拟机　　
