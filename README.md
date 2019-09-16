
# [iOS APP超级签名平台如图 

非市面上的linux打包

![扫码 获取超级签名非代理](https://raw.githubusercontent.com/iminvoker/superSign/master/IMG_2425.PNG "扫码 获取超级签名  非代理")
![扫码 获取超级签名非代理](https://raw.githubusercontent.com/iminvoker/superSign/master/IMG_2426.PNG "扫码 获取超级签名  非代理")


超级签名的优点就是非常稳定，不会像企业证书签名容易掉签问题，而且不用信任，安装后直接可以启动！追求稳定的很适合！
![QQ%E5%9B%BE%E7%89%8720190822105310.png](https://segmentfault.com/img/bVbwMar?w=740&h=223 "QQ%E5%9B%BE%E7%89%8720190822105310.png")

超级签名技术流程图

![17754767-5232c3f381b95597.png](https://segmentfault.com/img/bVbwMah?w=661&h=301 "17754767-5232c3f381b95597.png")

超级签名技术细节原理

简单来说，就是把添加苹果设备udid然后打包进行真机测试的过程（如下面真机测试教程），实现了自动化！

[申请ad hoc证书打包iOS真机测试教程](http://www.applicationloader.net/blog/zh/2514.html)

整体运行流程

1.用户手机安装预留的描述文件，获取本机udid后，向服务器返回用户的udid

2.服务器收到UDID后，将UDID添加到开发者账号下。

3.然后生成此udid签名用的证书描述文件，把预留的ipa重签。

4.重签后的iPA上传分发服务器，通过分发链接让用户下载。

使用配置文件获取UDID过程

苹果公司允许开发者通过IOS设备和Web服务器之间的某个操作，来获得IOS设备的UDID！

1.制作获取设备udid的描述文件.mobileconfig

2.用户安装.mobileconfig描述文件！

3.返回接收用户的udid数据，比如：UDID，需要在.mobileconfig描述文件中配置好，以及服务器接收数据的URL地址；


需要超级签名  立即扫码  非代理

![扫码 获取超级签名  非代理](https://raw.githubusercontent.com/iminvoker/superSign/master/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202019-08-26%20%E4%B8%8B%E5%8D%888.44.41.png "扫码 获取超级签名  非代理")




