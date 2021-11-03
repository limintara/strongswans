	StrongSWANS并非strongswan.org，是一个使用strongswan+freeradius+daloradius+whmcs搭建的科学上网平台,并实现了用户自主注册订阅(包含免费订阅)。StrongSWANS节点服务器采用IKEv2协议。关于常见VPN协议对比见下图：
![在这里插入图片描述](https://img-blog.csdnimg.cn/efdcd717da0848eab5b2401bd71ea89e.png?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5YiY5by66KW_5ZOl5ZOl,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)
以下是从网上截取的一段对IKEv2的说明：



> IKEv2有着非常实用的自动重连特性，当用户暂时失去互联网连接（比如进出火车隧道）的时候，它会自动重新建立VPN连接。对于手机用户来说确实是喜大普奔。Ikev2能跑在几乎所有iOS定制的VPN应用上，为了那些使用苹果公司官方VPN
> API的人无需越狱来使用它（也正因为这些优势，能让VPN供应商能够很容易地把更新配置文件推送到使用VPN的用户或者应用程序上）。   
> 比PPTP，SSTP和L2TP更快，它不涉及在点对点协议（Point-to-Point protocols，PPP）上的开销 非常稳定 -
> 尤其是切换网络或者在短暂的网络连接丢失之后重新连接的时候 非常安全 - 支持AES 128，AES 192，AES
> 256以及3DES加密算法 易于安装和配置 - 至少在用户端是如此 协议也支持黑莓的设备 暂时还不支持很多的平台
> 在服务器上搭建IKEv2相对来说很费劲，这也是很多问题的隐患所在 我们所对它的信任仅因为它进行了开源

所以IKEv2协议相比其他协议无疑是不错的选择，特别其断线可以自动重连的特性，很好的解决了wifi网络和移动流量网络切换时短暂的网络中断问题。

普通使用者看这里(如何从StrongSWANS获取科学上网账户以及各种设备配置)：
1，获取科学上网账户见如下视频:

2，免费订阅后进入用户中心查看用户名和密码已经可用节点信息：
![在这里插入图片描述](https://img-blog.csdnimg.cn/220cff97e8244375b9cdbbf5ddb84240.png?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5YiY5by66KW_5ZOl5ZOl,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)

![在这里插入图片描述](https://img-blog.csdnimg.cn/f045dd40f05b4b32b08e50b31d5023ee.png?x-oss-process=image/watermark,type_ZHJvaWRzYW5zZmFsbGJhY2s,shadow_50,text_Q1NETiBA5YiY5by66KW_5ZOl5ZOl,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)

3，window7及其以上版本操作系统配置步骤：
视频教程以windows11为例，windows7及以上操作系统配置类似。



