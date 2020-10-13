# Twirp

### 怎么运用的？
- 在.proto文件中定义好需要的服务，通过插件自动生成客户端、服务端的代码，然后编写业务逻辑。

### 自己的理解？
- 一个rpc框架，方便实现微服务，自动化生成客户端、服务端代码，专注于逻辑开发。
    - rpc:一个节点请求另一个节点，实现通信。
- twirp与gRPC的区别
    - gRPC只支持HTTP/2协议，twrip还支持HTTP1.1协议
        - HTTP1.1：keep-alive减少开销
        - HTTP2.0：多路复用一个TCP
    - gRPC自己实现了一套http服务器和网络传输层；twirp使用的是标准库net/http
    - twirp支持json格式数据交互