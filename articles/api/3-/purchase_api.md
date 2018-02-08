# 怎么在用友APILink商店购买和测试商品

以“企业工商信息查询”为例：

步骤一：使用友户通账号登录用友APILink（https://api.yonyoucloud.com）

步骤二：在页面找到“企业工商信息查询”商品，点进去。

![](/articles/api/3-/images/image1.png)
 

步骤三：点击购买。

![](/articles/api/3-/images/image2.png)

 
步骤四：选择一个适合的套餐，勾选“已阅读购买协议”后，点击“提交订单”

![](/articles/api/3-/images/image3.png)

 

步骤五：订单确认无误后，点击“去支付”。

![](/articles/api/3-/images/image4.png)

 

支持多种支付方式，如企业网银、信用卡、储蓄卡以及支付宝和微信

![](/articles/api/3-/images/image5.png)

 
步骤六：订单支付成功后，在下图页面中，点击“查看我的API”。

![](/articles/api/3-/images/image6.png)

 
步骤七：在“我的API”下找到刚刚购买的API，点击测试。

![](/articles/api/3-/images/image7.png)

 
步骤八：在“服务操作”栏选择“企业基本信息模糊查询”；参数值自己随便填写一个企业名称，我这里填写的“用友网络”；填写完毕后，点击“测试”。

![](/articles/api/3-/images/image8.png)

 
步骤九：在“测试”下方的“响应体”栏目会出现很多结果，选择自己想要进一步查询的一条数据，将“id”号复制。

![](/articles/api/3-/images/image9.png)

 
步骤十：在同一个页面中，服务操作选择“企业基本信息精准查询”，将刚刚复制的id号填入到“参数值”下面一栏中后，点击测试。

![](/articles/api/3-/images/image10.png)

 
步骤十一：页面下方的“响应体”会重新响应，出现的结果即查询到的最终结果。

![](/articles/api/3-/images/image11.png)

 
测试至此结束。
