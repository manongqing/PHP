---
解决端口号冲突的问题
---
默认情况下，所有网址的端口号均为 **80** 端口。
举个例子：www.baidu.com  和  www.baidu.com`:80` 均能访问到同一网站。

若出现端口号被占用问题，解决方式有两种：

1.开始->运行->cmd,输入 netstat -a -o ，点击回车, 查看端口号为80的进程所对应PID号。
打开任务管理器，查看进程的详细信息，找到对应的pid号，（如果不能找到或者发现为系统任务，则此端口号为系统所占用，不能采取这种解决方式，跳转第二种），
![](http://i.imgur.com/G4vfQ7X.jpg) 


![](http://i.imgur.com/ZEZ6IBw.jpg)


2.如果遇到系统占用80端口号的问题，就需要采取这种方法啦！

如果你用的是php的环境`wampsever`，左键点击，找到`Apache->httpd.conf`,进入后`ctrl+f`，输入`:80` ,找寻到端口后，将其改为`：81`，之后访问时在网址后加`：81`即可。
![](http://i.imgur.com/6ueoSDC.jpg)#  #

![](http://i.imgur.com/0LBvG2w.jpg)

---
![](http://i.imgur.com/oFTgzEt.jpg)

---

7/28/2016 1:26:33 PM 
by：晴