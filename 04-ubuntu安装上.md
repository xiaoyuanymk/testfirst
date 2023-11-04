# ubuntu安装上

## VMware安装及使用

```
VMware（虚拟机）是指通过软件模拟的具有完整硬件系统功能的、运行在一个完全隔离环境中的完整计算机系统，它能在Windows系统上虚拟出多个计算机，每个虚拟计算机可以独立运行，可安装各种软件与应用等。
```
1. 把安装程序**放到桌面** *（~放在英文路径下即可）*，以**管理员身份打开**，进入安装向导界面，点击下一步


![image-20200702154955191](04-ubuntu安装上.assets/image-20200702154955191.png)

2. 自定义安装，如下配置，点击下一步

![image-20200702155522289](04-ubuntu安装上.assets/image-20200702155522289.png)

3. 开始安装，等待完成

![image-20200702155628380](04-ubuntu安装上.assets/image-20200702155628380.png)

4. 安装完成，输入许可证

![image-20200702155808119](04-ubuntu安装上.assets/image-20200702155808119.png)

![image-20200702155855741](04-ubuntu安装上.assets/image-20200702155855741.png)

![image-20200702160016029](04-ubuntu安装上.assets/image-20200702160016029.png)

5. 重启电脑

### 注意:

>目前电脑更多的是从BIOS中查看是否支持虚拟化技术，当CPU支持VT-x虚拟化技术的前提条件下，部分电脑将自动开启VT-x功能，譬如IdeaPad Y450产品就采用了此设计。而大部分机型需要通过BIOS Setup界面手动进行设置，且默认情况下该选项为禁用状态。
[链接](http://robotrs.lenovo.com.cn/ZmptY2NtYW5hZ2Vy/p4data/Rdata/Rfiles/726.html)

## ubuntu镜像获取

### 镜像下载
[阿里云官方镜像站]()

![image-20200702161533986](04-ubuntu安装上.assets/image-20200702161533986.png)

### 课程资料镜像位置

```
AliOS Things物联网操作系统\day01\02-软件安装包\02-ubuntu16.4
```

## Ubuntu镜像安装

1. 打开VMware，创建新的虚拟机，选择自定义，点击下一步

![image-20200702161833038](04-ubuntu安装上.assets/image-20200702161833038.png)

2. 选择镜像位置，点击下一步

![image-20200702162051594](04-ubuntu安装上.assets/image-20200702162051594.png)

3. 配置名称，密码，点击下一步*（尽量简单，比如密码设置为1）*

![image-20200702162225250](04-ubuntu安装上.assets/image-20200702162225250.png)

3. 配置虚拟机名称，选择虚拟机安装路径*（安装路径应该选择空间大的磁盘进行，比如G盘，创建VMware/01-system文件夹）*，点击下一步

![image-20200702162444991](04-ubuntu安装上.assets/image-20200702162444991.png)

4. 配置虚拟机处理器个数

   > 参考博客，确定自己计算机的处理器个数

   ​	[VMWare中的处理器数量和每个处理器的内核数量概念及查询方法](https://blog.csdn.net/p1279030826/article/details/103044840)

![image-20200702163054803](04-ubuntu安装上.assets/image-20200702163054803.png)

5. 配置虚拟机内存个数（*我的内存是16G，分配8个给虚拟机）*

![image-20200702163337320](04-ubuntu安装上.assets/image-20200702163337320.png)

6. 配置网络类型（使用NAT模式，最简单使用）

![image-20200702163434893](04-ubuntu安装上.assets/image-20200702163434893.png)

7. 创建虚拟磁盘

![image-20200702163654384](04-ubuntu安装上.assets/image-20200702163654384.png)

![image-20200702163826608](04-ubuntu安装上.assets/image-20200702163826608.png)

8. 进入ubuntu界面

- 磁盘创建中

![image-20200702163902254](04-ubuntu安装上.assets/image-20200702163902254.png)

- 进入ubuntu界面

![image-20200702163938635](04-ubuntu安装上.assets/image-20200702163938635.png)

- 拷贝安装所需文件

![image-20200702164004425](04-ubuntu安装上.assets/image-20200702164004425.png)

- 确保本机能够连接外网*（需要在线下载......）*
![image-20200702164725350](04-ubuntu安装上.assets/image-20200702164725350.png)

9. 安装完成进入登录界面

![image-20200702165739562](04-ubuntu安装上.assets/image-20200702165739562.png)

10. 修改超级管理员密码

> 参考linux命令参考

​		[Linux 命令大全](https://www.runoob.com/linux/linux-command-manual.html)

```shell
lzd@ubuntu:~$ sudo passwd
[sudo] password for lzd: 
Enter new UNIX password: 
Retype new UNIX password: 
passwd: password updated successfully
```

![image-20200702170312266](04-ubuntu安装上.assets/image-20200702170312266.png)

11. 关机

- 关机

![image-20200702170517341](04-ubuntu安装上.assets/image-20200702170517341.png)

- 

12. 关闭启动时连接

![image-20200702172021145](04-ubuntu安装上.assets/image-20200702172021145.png)

13. 再次启动ubuntu

![image-20200702172208093](04-ubuntu安装上.assets/image-20200702172208093.png)