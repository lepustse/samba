# samba
以前我们在windows上共享文件的话，只需右击要共享的文件夹然后选择共享相关的选项设置即可。然而如何实现windows和linux的文件共享呢？这可以用到`samba`服务了。

## 应用场合
虚拟机与主机之间的文件传输

## 如何使用？
### 下载
`git clone https://github.com/neverxie/samba.git`

### 安装samba
`sudo apt install samba`

### 配置文件
`sudo cp ./smb.conf /etc/samba/smb.conf`

### 增加用户
`sudo smbpasswd -a`
> 温馨提示：samba用户密码设置与本系统密码一致较为方便
