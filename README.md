# samba
samba配置文件

## 1、介绍
以前我们在windows上共享文件的话，只需右击要共享的文件夹然后选择共享相关的选项设置即可。然而如何实现windows和linux的文件共享呢？这可以用到`samba`服务。

### 1.1、平台
Ubuntu

## 2、应用场合
虚拟机与主机之间的文件传输

## 3、下载与安装
### 3.1、下载
`git clone https://github.com/neverxie/samba.git`

### 3.2、安装samba
`sudo apt install samba`

### 3.3、配置文件
`sudo cp ./smb.conf /etc/samba/smb.conf`

### 3.4、samba重启生效
`reboot`

## 4、使用

### 4.1、添加用户
`sudo smbpasswd -a`
> 温馨提示：samba用户密码设置与本系统密码一致较为方便

### 4.2、windows设置
1. 添加一个网络位置，如图所示：
![1.png](./figure/1.png)
![2.png](./figure/2.png)
![3.png](./figure/3.png)

2. 指定网站的位置，如图所示：
本机ip+个人文件夹
![4.png](./figure/4.png)
![5.png](./figure/5.png)

3. 添加完毕，如图所示：
![6.png](./figure/6.png)
