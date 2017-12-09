### URI

#### 作者：Windson Yang

URI的全称是统一资源标识符（Uniform Resource Identifier），每一个URI对于一个系统来说都是唯一的，它有点像电话号码，电话号码在特定的国家内它是唯一的。而URI则在特定的范围内是唯一的，这个范围根据URI所使用的协议不同而不同，我们常见的两种URI包括一种是文件目录，另外一种是URI

#### 文件目录
    你可以尝试把电脑中的普通文件拖进浏览器，浏览器的地址栏会显示类似

    file:///Users/windson/EngineGirls/basic_tutorial/README.md
它就代表这个文件在你的电脑中的地址，它包含了使用的file协议，以及该文件的绝对路径

#### URI
这个大家一定接触过，就是我们常见的网址

    https://www.enginegirls.com/hello-world/
    
URI的完整形式就像这样：

    协议:[//[用户名[:密码]@]子域名.域名[:端口]][/路径][?参数][#定位]

其中[]里面的是可选的，也就是说用户名／密码／端口／路径／参数／定位这几个都是可选的。一个完整的URI例子是：

    https://username:password@enginegirls.com:80/hello-world/?id=100#hello

> URL是一种URI，它标识一个互联网资源，并指定对其进行操作或取得该资源的方法。可能通过对主要访问手段的描述，也可能通过网络“位置”进行标识。例如，http://www.wikipedia.org/这个URL，标识一个特定资源（首页）并表示该资源的某种形式（例如以编码字符表示的，首页的HTML代码）是可以通过HTTP协议从www.wikipedia.org这个网络主机获得的。（维基百科）

其他的URI包括：

    # ftp传输
    ftp://www.apple.com/resource.txt
    # 邮件协议
    mailto:Engine.Girls@example.com
