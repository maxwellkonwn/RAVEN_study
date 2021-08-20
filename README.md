# RAVEN_study
study for RAVEN
## Install Results

### on Windows
Windows下安装一切正常
### on linux
linux下安装颇有波折

#### Manjaro
1.Manjaro下似乎安装编译失败（报错），测试 test --j2 全报错  回顾官网为ubuntu环境下编译，故改用Kubuntu
#### Kubuntu
2.Kubuntu基于ubuntu，采用KDE Plasma桌面环境，易于配置美化
3.Kubuntu下几经波折，成功编译测试

## Win+Kubuntu 双系统准备
（建议可在虚拟机上先试试看）
### Kubuntu 系统盘制作 
在清华镜像源下载iso镜像，
然后推荐rufus制作启动盘，默认即可
### Windows 磁盘压缩
按照教程为Kubuntu留下足够磁盘空间即可

英特尔快速存储应该要关掉
### 双系统安装
1.进入BIOS（dell F12), 安装Kubuntu
2.Kubuntu 分区设置 /boot ~500M /swap似乎没有选项（后来安装好后查看自动分配了2G）/home可以大一点（似乎很大软件默认放在这了，如Anaconda /home/user/anaconda3）
/root 也可以大一点
3.其他设置似乎可以按默认
4.可能会遇到驱动问题（待补充）
5.可能会遇到硬盘格式问题（每次切换系统时需要进入BIOS更换磁盘类型，可以解决）
6.可能会遇到时间问题（待解决）

### Kubuntu设置
1.更新源（清华、USTC）

2.更新系统和软件

3.Gooogle chrome 插件下载（FQ、Github）,帐号同步

4.zsh/oh-my-zsh

### Anaconda

1.清华镜像源下载.sh

2.install  默认即可  注意 /home 不够大 在安装过程中指定安装路径

3.conda 换源

4.conda添加到.zshrc路径

5.anaconda3目录权限调整（chown - R username installpath ）

### pip

1.pip换源（参见清华镜像官网）

2.这一步很重要，不然部分包下载速度超级慢

