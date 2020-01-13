# BuildLocalUbuntu


# 如何本地ubuntu

参考：https://blog.csdn.net/lcuwb/article/details/82885920

具体：  


1.安装wsl

装openssh


https://blog.csdn.net/xiao_yuanjl/article/details/79147314

sudo apt-get remove openssh-server

sudo apt-get install openssh-server



2.设置root账号密码：



vi /etc/ssh/sshd_config
3.Port 2222   #设置ssh的端口号, 由于22在windows中有别的用处, 尽量不修改系统的端口号
PermitRootLogin yes   # 可以root远程登录
PasswordAuthentication yes     # 密码验证登录
AllowUsers root # 远程登录时的用户名

4.用pycharm连接wsl，进行编程




1. 以后的连接:
进入wsl
 sudo service ssh --full-restart
 
 
 然后xshell连接即可.
 
