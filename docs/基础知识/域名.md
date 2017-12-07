### URI

#### 作者：Windson Yang

URI的形式就像这样：

    协议:[//[用户名[:密码]@]子域名.域名[:端口]][/路径][?参数][#定位]


其中[]里面的是可选的，也就是说用户名／密码／端口／路径／参数／定位这几个都是可选的。我们最常见的一种URI就是URL，也就是网页资源的链接。

    https://www.apple.com/cn/environment/

其他的URI类型包括：

    # ftp传输
    ftp://www.apple.com/resource.txt
    # 文件协议
    file:///home/user/file.txt
    # 邮件协议
    mailto:John.Doe@example.com

https://www.apple.com/cn/environment/, 这个URL指向的地址就代表apple服务器一个资源地点，这个资源可能包括

1. 数据库查询相对应的资料，有可能包括现在访问的用户的头像，资料。
2. 要加载的样式，脚本，图片，文字

当你在浏览器输入这个URL，然后回车，浏览器会在域名解析之后把URL发给服务器，服务器就像一个大仓库，里面有很多小盒子，会根据传过来的目录（/environment/）然后查找到对应的盒子，然后把盒子的内容返回给浏览器。浏览器会根据返回的内容渲染，显示。例如如果它接收到服务器回复的：

    <img src="www.apple.com/iPhoneX-64" />

它知道这个标签代表这是一张图片，会先计算它的尺寸，然后再请求里面包含的图片的地址，再显示在浏览器界面中。
