# taotao-dubbo 基于dubbo实现的商城网站

## 一、项目背景
* 淘淘网上商城是一个综合性的B2C平台，类似于京东商城，天猫商城。会员可以在商城浏览商品、下订单，以及参加各种活动
* 管理员、运营可以在平台后台管理系统中管理商品、订单、会员等。
* 客服可以再后台管理管理系统中处理用户的询问以及投诉

## 二、淘淘商城架构
### 1.功能列表
![](https://www.showdoc.cc/server/api/common/visitfile/sign/8cc626bc4ecb9e7383f43734e9fff8dc?showdoc=.jpg)
* 后台管理系统: 管理商品、订单、类目、商品规格属性、用户管理以及内容发布等功能。
* 前台系统：用户可以再前台系统中进行注册、登录、浏览商品、首页。下单等操作。
* 会员系统：会员可以在该系统中查询已下的订单、收藏的商品、我的优惠券、团购等信息。
* 订单系统： 提供下单、查询订单、修改订单状态、定时处理订单。
* 搜索系统： 提供商品的搜索功能。
* 单点登录系统： 为多个系统之间提佛那个用户登录凭证以及查询登录用户的信息。

### 2.淘淘商城系统架构--基于SOA的架构体系
![](https://www.showdoc.cc/server/api/common/visitfile/sign/64b103b0f2f5057c706d7bf97a612bd2?showdoc=.jpg)

* 注：架构演变可参考博文：https://blog.csdn.net/josblue/article/details/80923945

### 3.工程搭建
![](https://www.showdoc.cc/server/api/common/visitfile/sign/cfe4c6b0dedb2ac422899c8c636d0fb4?showdoc=.jpg)

* 注：使用ideal搭建工程可参考博文：https://blog.csdn.net/josblue/article/details/80924006

## 三、开发环境
* 系统环境：Win10
* IDE工具：ideal2017.3.4 
* 数据库： Mysql5.5
* 服务器：tomcat8.0

## 四、使用技术
* 后端框架：Spring+SpringMVC+mybatis
* 后台管理系统框架：EasyUI
* 服务中间件：dubbo+zookepper
* 消息队列：Activemq
* 数据库中间件： mycat
* 其他：FastDFS图片上传，freeMarker模板引擎，redis数据缓存，Quartz定时任务，solr搜索服务，keepalived+nginx实现高可用等
