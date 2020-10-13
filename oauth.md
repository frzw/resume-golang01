# oauth

### 怎么使用的？
- 再数据提供端和数据使用端之间加上一层权限校验的机制，存储数据之前通过接口获取token，存储的时候要带上这个token才能成功。

### 自己的理解？
- 授权的开放网络标准，用来授权第三方应用，获取用户的数据
- 流程
```
(A). 用户打开客户端(Client)，客户端向授权服务器(Resource Owner)发送一个授权请求
 (B). 用户同意给客户端(Client)授权
 (C). 客户端使用刚才的授权去向认证服务器(Authorization Server)认证
 (D). 认证服务器认证通过后，会给客户端发放令牌(Access Token)
 (E). 客户端拿着令牌(Access Token)，去向资源服务器(Resource Server)申请获取资源
 (F). 资源服务器确认令牌之后，给客户端返回受保护的资源(Protected Resource)
```