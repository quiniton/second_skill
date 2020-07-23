### 高并发秒杀系统：SpringBoot+Mybatis+Redis+RocketMq 

感谢这位博主：https://github.com/hfbin/Seckill（基于上面进行优化）

---
### 项目启动说明
> 1、启动前，进行相关redis、mysql、rocketMq地址   
2、登录地址：http://localhost:8888/page/login      
3、商品秒杀列表地址：http://localhost:8888/goods/list   
4、账号：18077200000，密码：123456   
   
---

### 其它说明
1、数据库共有一千个用户左右（手机号：从18077200000~18077200998 密码为：123456），为压测准备的。（使用 UserUtil.java该类生成的，生成token做压测也是在此类里面）    
2、此项目共有两个分支，master分支只是完成了秒杀的所有业务逻辑功能，并没有优化。V2.0分支做了优化如下：   
    1)、页面缓存、商品详情静态化、订单静态化（感兴趣可以把所有页面都做静态化）
    2)、加入消息队列RabbitMQ，对秒杀接口进行优化。
    3)、隐藏秒杀接口地址
    4)、接口限流防刷
    5)、解决超卖问题


---
### 页面截图
登录页
![123](img/1.png)

商品列表情页
![123](img/2.png)

商品详情页
![123](img/3.png)

订单详情页
![123](img/4.png)

---
