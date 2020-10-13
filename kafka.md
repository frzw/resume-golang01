# kafka

### 怎么使用的？
- 爬虫框架状态监控，应用的是日志同步功能，状态机端日志消费端，爬虫框架是日志采集端。

### 自己的理解？
- 分布式处理流系统，可以像消息队列一样分布和订阅消息。将消息存储在topic,topic包含键值和时间戳。分布式提供了容错性，并发处理消息的机制
- topic、producer、consumer、partition、broker、consumer group、offset。
- 启动zookeeper,再启动kafka,创建topic,向topic发消息，向topic消费消息。