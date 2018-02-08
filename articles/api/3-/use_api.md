# 开发人员怎么调用APILink购买的接口

以企业工商信息查询为例：

如下图，开发者可以在API详情页面中看到java调用demo,curl,php以及.net的demo，只需将apicode和url替换成需要调用的api即可。目前demo只提供apicode认证，（AppKey和Appsecret的验签调用另行说明）

![](/articles/api/3-/images/image12.png)



 
此外,对于目前使用场景最多的java调用我们封装了sdk，可以直接集成(提供了两种认证方式调用)。

步骤一：在购买完api后，进入使用者门户-〉sdk文档java下载，如下图

![](/articles/api/3-/images/image13.png)


 

步骤二：解压缩下载下来的dysmsapi_demo_sdk__java.zip文件

![](/articles/api/3-/images/image14.png)


 
步骤三：.在eclipse中新建Java Project项目

![](/articles/api/3-/images/image15.png)


 
步骤四：导入项目jar包，在解压后的sdk文件夹找到lib打开，导入iopv_apilink.jar

(注：源码下载https://github.com/qingfengtanying/APIHttpInvoker.git)

![](/articles/api/3-/images/image16.png)

![](/articles/api/3-/images/image17.png)
 
 
步骤五：导入其它依赖jar包，如果不用Maven,所有依赖jar包都在 relyOnLib文件夹中，直接导入项目即可。

![](/articles/api/3-/images/image18.png)


 
步骤六.新建test包

![](/articles/api/3-/images/image19.png)


 
步骤七.打开javaSDK文件夹。将所有api的java文件粘贴到test包下

![](/articles/api/3-/images/image20.png)


 
步骤八.导入HttpClient.properties配置文件，此配置文件为线程池参数文件

![](/articles/api/3-/images/image21.png)


 
步骤九.打开api文件，修改propertyUrl。此参数是配置HttpClient.properties文件路径（注：示例代码中出现”*******”替换的参数）

![](/articles/api/3-/images/image22.png)


 
步骤十.修改apicode。目前验证方式有apicode和appkey两种安全验证，其中appkey做了sha数字验签, 根据验证方式修改如下代码：

![](/articles/api/3-/images/image23.png)


 
如下图Apicode以及appkey在使用者门户－〉我的api中找到

![](/articles/api/3-/images/image24.png)


 
步骤十一.修改调用api的header和表单参数参数

![](/articles/api/3-/images/image25.png)


 
启动main函数测试
