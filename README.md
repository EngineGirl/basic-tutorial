# 基础入门

- 加入社区（可选)
    - 关注EngineGirls公众号
    - 公众号留意报名参加编程培训

- 编程前准备

    - [注册Github](#注册Github)
    - [创建公钥](#创建公钥)

    - [下载软件](#下载软件)

    - [选择编辑器](#选择合适的编辑器)
    - [科学上网](#科学上网)

- 计算机基础知识

    - [终端](#终端)
    - [路径](#路径)
    - [字符串编码](#字符串编码)



## 注册Github

一个拥有过百万名开发者的社区。

这个星球上最流行的开源托管服务。目前已托管超过400万个编程项目。

我们将通过Github将我们的教程，习题和代码托管在云端。第一步注册Github
  
  https://github.com/join?source=header-home
  


![1](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/img/github_1.jpeg)

![2](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/img/github_2.jpeg)

![3](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/img/github_3.jpeg)


注册成功后需要创建公钥。

## 创建公钥(https://gist.github.com/yisibl/8019693)

1. 首先启动一个Git Bash窗口（非Windows用户直接打开终端）

2. 执行：
    
    >cd ~/.ssh

    如果返回“… No such file or directory”，说明没有生成过SSH Key，直接进入第4步。否则进入第3步备份。

3. 备份：

   >mkdir key_backup
   mv id_isa* key_backup

4. 生成新的Key：（引号内的内容替换为你自己的邮箱）

   >ssh-keygen -t rsa -C "your_email@youremail.com"

  输出显示：

    >Generating public/private rsa key pair. Enter file in which to save the key 
    (/Users/your_user_directory/.ssh/id_rsa):<press enter>

  直接回车，不要修改默认路劲。

    >Enter passphrase (empty for no passphrase):<enter a passphrase>
    Enter same passphrase again:<enter passphrase again>

  设置一个密码，在每次远程操作之前会要求输入密码！觉得麻烦的话可以直接回车跳过。

5. 成功：

    >Your identification has been saved in /Users/your_user_directory/.ssh/id_rsa.
    Your public key has been saved in /Users/your_user_directory/.ssh/id_rsa.pub.
    The key fingerprint is:
    ... ...

6. 提交公钥：

   6.1 找到.ssh文件夹，用文本编辑器打开“id_rsa.pub”文件，复制内容到剪贴板。
   
   6.2 打开 https://github.com/settings/ssh ，点击 Add SSH Key 按钮，粘贴进去保存即可。

## 下载软件
### Git下载

    # Windows64位
    https://npm.taobao.org/mirrors/git-for-windows/2.12.0.windows.1/Git-2.12.0-64-bit.exe
    # Windows32位
    https://pan.baidu.com/s/1dElvwtV
    # 苹果系统
    https://git-scm.com/download/mac

    # 如果git下载太慢，可以使用这个地址下载（第一个是64位）
    https://npm.taobao.org/mirrors/git-for-windows/2.12.0.windows.1/Git-2.12.0-64-bit.exe
    https://pan.baidu.com/s/1dElvwtV

### Python下载（在Python 3.5.3 - 2017-01-17下）

    # Windows
    https://www.python.org/downloads/windows/
    32位选择
    Download Windows x86 executable installer
        
    64位选择
    Download Windows x86-64 executable installer
    
    # 苹果系统
    https://www.python.org/downloads/mac-osx/

## 选择合适的编辑器
学员如果之前有编程基础，可以自行选择熟悉的代码编辑器。

零基础学员推荐（atom编辑器）访问
    https://atom.io/

下载安装

## 科学上网

hosts文件是一个特别的文件，在电脑访问网站的时候会先在hosts文件找对应的ip地址。
例如如果你要访问google.com, 系统会先查询google.com在hosts文件中有没有对应的ip地址，如果有的话直接访问此ip地址:

    56.44.223.55 google.com

这样我们就可以部分绕过DNS污染访问网站了

### 获取最新hosts文件
    
    https://raw.githubusercontent.com/racaljk/hosts/master/hosts

### 替换旧的文件

hosts所在文件夹：

Windows系统 

    C:\Windows\System32\drivers\etc\hosts

Mac系统 

    /etc/hosts
Linux系统 

    /etc/hosts

### 刷新DNS缓存
- Windows

>开始 -> 运行 -> 输入cmd -> 在CMD窗口输入

>ipconfig /flushdns

- Linux

>终端输入

>sudo rcnscd restart

### 访问google.com

## 终端
现代的个人电脑通常都会配有图形化界面，也就是说假如你要删除一个文件，可能会先找到这个文件，然后把它拖到回收站，不过你也可以通过直接输入指令的方式删除。Windsows7或之后的版本大家可以使用Powershell：

    Windows 7：打开 开始 菜单，在搜索框里输入 powershell，点击结果里的 Windows Powershell。

    Windows 8+：win + Q，搜索 powershell。

删除文件的指令是：

    # Windsons
    Remove-Item [FilePath]
    # OSX
    rm [FilePath]


编程会经常接触终端，因为我们的指令都需要在终端中输入，或者保存在文件，然后由终端执行，例如要计算7的25次方：

方法一：

1. 终端中输入python
2. 输入7**25 回车

方法儿：

1. 新建一个以py为后缀的文件，例如cal.py
2. 文件中输入print(7**25) 保存，回车
3. 在终端直接输入python cal.py 

以上两个方法都可以得到答案1341068619663964900807，当然如果是这类计算一般可以是用系统自带的计算机，不过假如要读取数据，或者做一些文件处理，定时任务的话，那就必须使用终端啦。

## 路径
当你打开终端的时候，会看到例如：

    Windsons
    C:\Administor\foo\:

    OSX
    WindsondeMacBook-Air:~

（这篇文章中，统一使用windows的\，如果使用的是其它系统，只需要替换为\）

这样的字符在行首，这个就是当前执行指令的路径。也就是你的当前路径，那什么是绝对路径和相对路径呢？

举个现实生活的例子：
你在路上遇到你的好朋友李会玩，她问你的公司地址在哪里，你可能有两种答案：

1. 中国广东省广州市思哲路石室大厦 
2. 以这里为起点，西南方向500米的石室大厦 

第一个答案从国家到省份城市全部巨细无遗地描述出来就相当于绝对路径， 第二个答案以当前的位置为起点所描述的就是相对路径。
例如：有个文件存放在

    C:\Administor\foo\test.txt

那么你要读取它可以直接读取这个路径

    with open('C:\Administor\foo\test.txt', 'r', encoding='utf-8') as f:
        txt = f.readlines()
你也可以根据当前自己的位置找这个文件，假如你打开终端，当前路径是

    C:\Administor\foo\:
那么你也可以这样读取 

    with open('test.txt', 'r', encoding='utf-8') as f:
        txt = f.readlines()

>相对路径地址 ＝ 绝对路径的地址－当前路径

    test.txt = C:\Administor\foo\test.txt - C:\Administor\foo\

 有些特殊的情况是.以及.. 这两个符号分别代表当前路径以及上一级目录，也就是说如果你当前路径是：
 
    C:\Administor\foo\
那么

    .\ = C:\Administor\foo\
    ..\ = C:\Administor\

问题来了，假如文件在

    C:\Administor\foo\test.txt
 
你当前路径为

    C:\Administor\foo\cherry\

要如何读取此文件呢？你既可以使用绝对路径的方式直接读取

    with open('C:\Administor\foo\test.txt', 'r', encoding='utf-8') as f:
        txt = f.readlines()

也可以
 
    with open('..\test.txt', 'r', encoding='utf-8') as f:
        txt = f.readlines()

其实意思就是返回上一层目录就是先到

    C:\Administor\foo
然后再读取文件

###如何在终端显示当前的绝对路径

    # Windows
    pwd

    # OSX
    pwd

###如何切换路径
可以使用cd指令

    cd [PATH]

这里的path既可以是绝对路径也可以是相对路径，如果当前路径为：

    C:\Administor\foo\:

你要跳到

    C:\whatever\sunkist\:
就可以

    cd C:\whatever\sunkist\
    # 或者
    cd ..\..\whatever\sunkist\

## 字符串编码
