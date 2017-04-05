# 基础入门

- 加入社区（可选)
    - 关注EngineGirls公众号
    - 公众号留意报名参加编程培训

- 编程前准备

    - [注册Github](#github)

    - [下载软件](#下载软件)

    - [选择编辑器](https://github.com/EngineGirl/basic-tutorial/blob/master/%E9%80%89%E6%8B%A9%E5%90%88%E9%80%82%E7%9A%84%E7%BC%96%E8%BE%91%E5%99%A8.md)
    - [科学上网]

3. 计算机基础知识

    - [终端]
    - [路径]
    - [字符串编码]



## Github

一个拥有过百万名开发者的社区。

这个星球上最流行的开源托管服务。目前已托管超过400万个编程项目。

我们将通过Github将我们的教程，习题和代码托管在云端。第一步注册Github
  
  https://github.com/join?source=header-home
  


![1](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/img/github_1.jpeg)

![2](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/img/github_2.jpeg)

![3](https://raw.githubusercontent.com/EngineGirl/basic-tutorial/master/img/github_3.jpeg)


注册成功后需要创建公钥。

## 如何创建公钥(https://gist.github.com/yisibl/8019693)

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

