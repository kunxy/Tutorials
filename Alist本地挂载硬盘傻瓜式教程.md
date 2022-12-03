以下是经由本人实操过程——  
操作系统Windows 11

### 下载

GitHub 上alist的安装地址: [https://github.com/alist-org/alist](https://link.zhihu.com/?target=https%3A//github.com/alist-org/alist)

![](https://pic2.zhimg.com/80/v2-e9e80db483ca8b103043d6df980b123d_720w.webp)

  

  

点击v3.1.0进入,滑到最底下选择[alist-windows-4.0-amd64.zip](https://link.zhihu.com/?target=https%3A//github.com/alist-org/alist/releases/download/v3.1.0/alist-windows-4.0-amd64.zip)这个版本下载

  

![](https://pic3.zhimg.com/80/v2-4e5a39aeff70e6445ce6ffe4234c4e06_720w.webp)

  

将刚下载好的[alist-windows-4.0-amd64.zip]解压，得到alist-windows-4.0-amd64.exe程序放到新的文件夹

### 安装Alist

在路径栏输入cmd

![](https://pic2.zhimg.com/80/v2-76e7e6c2c354d6d39309741c5dda0481_720w.webp)

  

拖拽到cmd，回车运行

![](https://pic1.zhimg.com/80/v2-6ea96acdeab192c671a62cb1a08e6bf8_720w.webp)

  

![](https://pic4.zhimg.com/80/v2-e18a5c4e243697ee19b31612c9613687_720w.webp)

  

链接服务器（下次重启，也是需要通过同样的步骤链接服务器）

继续输入：alist.exe server,回车

![](https://pic2.zhimg.com/80/v2-7a94897ec51cc987c1f0870f9f2ce105_720w.webp)

  

  

得到输出结果

![](https://pic1.zhimg.com/80/v2-6444941ea1e518493dad6d65b2dde648_720w.webp)

  

可以看到0.0.0.0:5244这串数字，后面的5244是服务器端口，前面的4个0是需要填本机的ip地址。(服务器地址：本机ip+端口)

### 查看本机IP地址：

1、使用Windows+R键打开“运行”窗口，然后输入CMD进入命令提示窗口

![](https://pic4.zhimg.com/80/v2-0ac8d84dfbaf1891a59e024b30bb21b7_720w.webp)

  

  

2、进入命令窗口之后，输入：ipconfig/all 回车即可看到本地链接IP4地址信息

![](https://pic4.zhimg.com/80/v2-f7a25d6316ae96434c85e3fac9790ccb_720w.webp)

  

192.168.0.108:5244是我进入服务器的ip地址,不要照抄我的，每个机子的ip段不一样。

### 查看Alist登录密码

同样的在路径栏进入cmd

![](https://pic4.zhimg.com/80/v2-b59924c87a1a777f3f14aa962291abdb_720w.webp)

  

  

输入：alist.exe password

![](https://pic3.zhimg.com/80/v2-6aee7ca905ec85809c5166b74cc5deb2_720w.webp)

  

  

输出结果看到账号和密码

![](https://pic4.zhimg.com/80/v2-10fbcb2c4b3d229c8bee2edec2a9e63b_720w.webp)

  

  

![](https://pic1.zhimg.com/80/v2-aa058f858dc5e48b5a1005667dbdccb4_720w.webp)

  

  

输入刚查到的账号和密码

![](https://pic1.zhimg.com/80/v2-8de2167bb6c5dbd7f1f4edaa6ce11bfc_720w.webp)

  

  

登录后点管理进入设置

![](https://pic1.zhimg.com/80/v2-6ab043f09755f02dc87d92e4d5bedd24_720w.webp)

  

  

![](https://pic1.zhimg.com/80/v2-e44826005a6286cb006e15423e2e0150_720w.webp)

  

  

![](https://pic2.zhimg.com/80/v2-88236f068cab470495a43f06f0100ea1_720w.webp)

  

  

我添加的是阿里云盘，以阿里云盘为例

![](https://pic2.zhimg.com/80/v2-65f69c2208109796fb7facb75f366bd1_720w.webp)

  

填写说明：  
挂载路径：设置的盘符（例：E/F/G），注：设置的盘符不能与本地已有的盘符冲突。  
刷新令牌：参见下文  
根文件夹ID：参见下文

其它选填参数：缓存过期时间可设置为0，设置为0不过期

  

![](https://pic4.zhimg.com/80/v2-cdd77401b7e745eb9f021d9cc4eaf887_720w.webp)

  

[Guide | AList文档 (nn.ci)](https://link.zhihu.com/?target=https%3A//alist.nn.ci/zh/guide/)

  

![](https://pic3.zhimg.com/80/v2-b775f63afe7b82ee04c47652f170713a_720w.webp)

  

  

[阿里云盘 | AList文档 (nn.ci)](https://link.zhihu.com/?target=https%3A//alist.nn.ci/zh/guide/drivers/aliyundrive.html)

### 获取(Token)令牌

  

![](https://pic2.zhimg.com/80/v2-a6455c7203c1f60d43a41111d5695b2d_720w.webp)

  

用手机阿里云盘APP扫码获取

  

  

得到令牌

  

这一步是查看根文件夹ID

![](https://pic4.zhimg.com/80/v2-3e61b57ed0a5b748ea07175fa96d4117_720w.webp)

  

  

填完后点击添加

![](https://pic4.zhimg.com/80/v2-3da29bcee8c8ba8901116b8b3c1213e3_720w.webp)

  

以上网页聚合已经做好了，但我们的目的是内容直接对应到本地硬盘，就需要用到一个软件RaiDrive。

### 安装RaiDrive

  

![](https://pic4.zhimg.com/80/v2-b2f1aea7b275c4b163b29739dfaf9f6b_720w.webp)

  

  

直接安装，安装过程中会检查安装环境组件，有弹窗安装环境组件的，全部点安装，一定要安装。

安装完后，打开软件可以看到这个界面，点击添加

![](https://pic2.zhimg.com/80/v2-7e74febd85b7a533e9b76877381bd745_720w.webp)

  

  

标注的地方跟着填

![](https://pic2.zhimg.com/80/v2-9181a7e95ffad36ca714de0003076f91_720w.webp)

  

最后点击链接，链接成功后挂载的本地文件夹会弹窗。

  

---

考虑到有些小伙伴可能没有注意看，故做一下补充说明：

开头步骤“alist.exe server,回车 ”，这个cmd是不能关的，关闭等于断开Alist局域网的链接，关闭就打不开了。

每次链接都要做这一步，只有局域网链接上，本地挂载的云盘才能正常访问。

![](https://pic2.zhimg.com/80/v2-07519bda7ed2b20dde10eb5812df2309_720w.webp)

上述步骤每次都要在程序目录文件夹打开觉得比较麻烦的话，有一个提高一点效率的方法

通过cmd命令快速打开Alist.exe的方法：

通过控制面板进入系统信息或通过在“我的电脑”右键属性进入

![](https://pic3.zhimg.com/80/v2-bd1257075d4205aecfb353d76b6a2ebe_720w.webp)

进入高级系统设置

![](https://pic2.zhimg.com/80/v2-a59c906b82766563c94ffc8427a0e2c9_720w.webp)

进入环境变量

![](https://pic4.zhimg.com/80/v2-9444470932798153c0f691a1f7e39ee7_720w.webp)

现在打开Alist.exe目录的所在文件夹，选中Alist.exe右键属性，复制程序路径

![](https://pic2.zhimg.com/80/v2-0a3e4a7dcb82d1a6d2e1e52ce96c1249_720w.webp)

回到环境变量，选中Path，点击编辑

![](https://pic1.zhimg.com/80/v2-438b325fc049788369f7279df3916f6c_720w.webp)

点击新建，粘贴刚刚复制的Alist.exe的程序路径，点击确定

![](https://pic4.zhimg.com/80/v2-ca50692803bb4b3002cf826ebcd1e13f_720w.webp)

下次要链接服务器只需要：

windown10/11比较方便的是按键盘上的win键打开开始菜单，输入cmd进入-输入alist.exe server

  

---

  

补增一个知友遇到的问题，希望对遇到同样问题的知友有帮助。

感谢知友提供的问题，问题以及解决方法如下：

  

![](https://pic4.zhimg.com/80/v2-c2881a0c7aaa69aa04ca70d641c7ff2f_720w.webp)

failed to start: listen tcp 0.0.0.0:5244: bind: Only one usage of eacch socket address (protoco

l/network address/port) is normally permitted.

遇到的问题是端口被占用，服务器无法启用。

  

需要杀掉占用的程序：

打开cmd,输入netstat -a -n -o,就会显示出使用端口的进程pid,然后在进程管理器中查看相应的进程,默认情况下windows的进程管理器是不显示pid的，你可以通过在[查看]->[选择列]中选种查看pid，然后进程查看器中就会显示pid了 目前发现有几个程序是有时会占用这个端口的:pplive,skype,或者在杀毒软件瑞星关闭了连接网络功能.

解决方法见原文链接：https://www.chinastor.com/apache/0G3332952016.html?mobile_redirection=false


---
使用bat文件实现alist.exe开机自启动:

在Alist目录新建一个txt文件，由于一开始已经做了添加环境变量这一步，所以直接打开编辑输入如下：

alist.exe server
保存后，文件后缀改为.bat






接下来关键一步，拷贝文件粘贴到Windows启动文件夹

1.按下windows+R 输入：shell:startup

2.把*.bat拷贝到此文件夹

OK。完成



补充：cmd 命令一直开着，最小化也怕误删了，我可以把它隐藏吗？
以下是bat脚本cmd命令执行后隐藏的方法：

开头

@echo off

if "%1" == "h" goto begin

mshta Vbscript:createobject("wscript.shell").run("%~nx0 h",0)(window.close)&&exit

:begin

+你要输入的命令。



例：

@echo of

if "%1" == "h" goto begin

mshta Vbscript:createobject("wscript.shell").run("%~nx0 h",0)(window.close)&&exit

:begin

alist.exe server
