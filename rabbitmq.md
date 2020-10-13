# rabbitmq

### 怎么使用的？
- gocron发出任务通过post请求celery,celery客户端开启爬虫任务请求，请求进入到rabbitmq消息队列，rabbitmq分发请求任务到celery服务端，celery处理请求进行python端的爬虫，python端爬虫完毕后通过grpc调用go端的爬虫处理，go爬虫端处理python端发来的爬虫数据，数据进行数据库的存入。
- rabbimq:分发任务、流量削峰、串行。

### 自己的理解？
- rabbitmq是高级消息队列协议的开源代理软件。应用场景有异步处理（串行、并行、异步）、应用解耦（淘宝订单）、流量削峰（抢红包）。