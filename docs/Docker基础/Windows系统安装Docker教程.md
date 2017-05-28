##Windows安装Docker教程
[官方英文教程](https://docs.docker.com/docker-for-windows/install/#download-docker-for-windows)

###安装前须知

你的系统需满足以下几个条件，如果不满足以下要求，请参考[第二节](#第二节)

- 确保你电脑安装了64位的Windows 10 Pro, Enterprise或者Education(1511 November update, Build 10586 or later)版本。

- 如果你的电脑安装了VirtualBox（一个虚拟机软件，默认系统没有安装）请注意，Windows的Docker版本因为需要Microsoft Hyper-V来运作，安装之后会令VirtualBox无效。

- 必须启动虚拟化（默认启动），可以在任务管理中找到这一项确保enabled

    Windows8检查

    点击开始 > 任务管理 > 性能 > CPU 

    ![windows-virtualization](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/imgs/install_docker/Windows/win-virtualization-enabled.png)
    
    黄色的Virtualization为Enabled即可

    Windows7检查

    运行[Microsoft® Hardware-Assisted Virtualization Detection Tool](http://www.microsoft.com/en-us/download/details.aspx?id=592)工具，然后按照步骤来检测。

>Docker建立的容器和镜像会被计算机上面的所有用户共享，多账号的系统中要注意数据安全问题。

###开始安装

1. 下载[Docker稳定版](https://download.docker.com/win/stable/InstallDocker.msi)
2. 双击下载文件夹中的InstallDocker.msi文件。
3. 阅读协议内容觉得没问题之后点击接受协议（不接受将无法安装:O)，然后安装。

>一般软件应该安装在非系统盘（C盘）中，这样即使以后需要重装系统，软件也不会丢失。安装路径不要包含中文）

4. 输入系统管理员密码使Docker可以安装网络组件。
5. 完成
![windows-docker-install-finished](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/imgs/install_docker/Windows/installer-finishes.png)

####启动Docker
安装完成后Docker会自动启动，你可以从状态栏看到Docker正在运作
![win-install-success-popup-cloud](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/imgs/install_docker/Windows/win-install-success-popup-cloud.png)
就这样愉快地结束了。

##第二节
如果不满足条件（例如你使用的是Windows7或者Windows8系统）我们需要安装另外一款工具来运行Docker

###安装前准备
- 先确保自己的Windows系统是Windows7以上（Windows7, Windows8，Windows10都可以）的64位系统，可以通过这里确定[Windows系统版本](https://support.microsoft.com/zh-cn/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64-bit-version-of-the-windows-operating-system)，如果不是64位的话请更新64位的系统。

- 必须启动虚拟化（默认启动），可以在任务管理中找到这一项确保enabled

    Windows8检查

    点击开始 > 任务管理 > 性能 > CPU 

    ![windows-virtualization](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/imgs/install_docker/Windows/win-virtualization-enabled.png)
    
    黄色的Virtualization为Enabled即可

    Windows7检查

    运行[Microsoft® Hardware-Assisted Virtualization Detection Tool](http://www.microsoft.com/en-us/download/details.aspx?id=592)工具，然后按照步骤来检测。


##开始安装

- 确保自己没有运行Virtual Box（默认系统没有按照这个软件）
- 点击右边链接下载[Docker Toolbox](https://download.docker.com/win/stable/DockerToolbox.exe)
- 下载完毕后双击安装，如果这时候系统问你是不是允许程序修改，点击Yes
- 选择默认选项直到安装完毕
