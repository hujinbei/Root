# 更改mac中root权限

* 首先输入在mac终端输入：

```
	sudo passwd root

```

* 然后输入新的密码，在重复输入刚刚设定的新密码；

* 再输入命令
```
	su
```

* 再次输入密码，便更改完成了

![](/Users/huhuhu/Desktop/sublime文件/权限更改/1.png)

更改完成后终端中的用户名发生了变化；

# 更改linux中root权限

* 首先在终端输入"sudo passwd -u root"，然后输入原有的linux密码；

* 再输入“sudo passwd root”，开始设置新的密码，然后再次输入新密码；

* 输入“su -”，输入新设置的密码，确认是否已经开启最高权限，根据终端的用户名显示为“root@+用户名+电脑型号”表示root权限已成功开启；

* 输入“exit”退出root权限登录；

![](/Users/huhuhu/Desktop/sublime文件/权限更改/root.png)

* 然后设置登录面板，使其实现root登录，

* 进入/usr/share/lightdm/lightdm.conf.d/

* 编辑: 50-unity-greeter.config

* 添加如下代码,保存退出

```

user-session=ubuntu
greeter-show-manuallogin=true
all-guest=false

```
![](/Users/huhuhu/Desktop/sublime文件/权限更改/root1.png)

# 更改windows中root权限

* 首先打开"开始"，在底部输入“cmd”，单击右键选择“以管理员身份运行（A）”，打开后便是最高权限运行；
![](/Users/huhuhu/Desktop/sublime文件/权限更改/3.png)

** 最高权限运行（访问系统文件）**

![](/Users/huhuhu/Desktop/sublime文件/权限更改/2.png)

** 普通权限运行（访问用户文件）**

![](/Users/huhuhu/Desktop/sublime文件/权限更改/4.png)
