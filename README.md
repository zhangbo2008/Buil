# BuildLocalUbuntu


# 如何本地ubuntu

参考：https://blog.csdn.net/lcuwb/article/details/82885920

具体：  


1.安装wsl
2.设置root账号密码：


3.Port 2222   #设置ssh的端口号, 由于22在windows中有别的用处, 尽量不修改系统的端口号
PermitRootLogin yes   # 可以root远程登录
PasswordAuthentication yes     # 密码验证登录
AllowUsers root # 远程登录时的用户名

4.用pycharm连接wsl，进行编程
