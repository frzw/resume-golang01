# gqlgen

### 怎么使用的？
- 在.graphql定义好跟.proto对应的服务，生成对应的服务方法，这些方法调用twirp的方法来实现方法，运行grapql的客户端进行测试。


### 
- gqlgen是用于构建graphql服务器的go库。
    - graphql:用于API的查询语言，有自己的引擎和语言，相当于数据库和SQL的关系。
    - graphql与rest的区别：
        - graphql:资源与获取方式分离，通过url主动获取想要的数据。
        - rest:每个资源都是url，被动获取想要的数据。