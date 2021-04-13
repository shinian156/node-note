## node 
   
[阮一峰Koa 框架教程](http://www.ruanyifeng.com/blog/2017/08/koa.html)

[Node.js 轻松学 基础篇 入门](https://github.com/able8/hello-nodejs)

[w3c](https://www.w3cschool.cn/nodejs/)

[廖雪峰](https://www.liaoxuefeng.com/wiki/1022910821149312/1101571555324224)

[libuv](http://luohaha.github.io/Chinese-uvbook/source/introduction.html)

























## 浅谈Node.js在携程的应用
docker搭建node环境   https://cloud.tencent.com/developer/article/1558725
浅谈Node.js在携程的应用 https://cloud.tencent.com/developer/article/1494576

node特点
https://cloud.tencent.com/developer/article/1476248


最佳实践

```
由nginx做接口转发、负载，

varnish做数据缓存层，

node是业务处理层
```


BigPipe是一个重新设计的基础动态网页服务体系。大体思路是，分解网页成叫做Pagelets的小块，然后通过Web服务器和浏览器建立管道并管理他们在不同阶段的运行。这是类似于大多数现代微处理器的流水线执行过程：多重指令管线通过不同的处理器执行单元，以达到性能的最佳。虽然BigPipe是对现有的服务网络基础过程的重新设计，但它却不需要改变现有的网络浏览器或服务器，它完全使用PHP和JavaScript来实现。


passport 登录认证

http://blog.fens.me/nodejs-express-passport/




### node

### 最佳实战

由nginx做接口转发、负载，varnish做数据缓存层，node是业务处理层，在4核服务器上启动4个node进程(跟cpu核数对应)，通过nginx的ip_hash做负载均衡，将请求均分给各个node进程，充分利用cpu的性能；node进程在收到请求后会通过内网调用发送http请求获取后端接口数据；varnish是一款高性能、开源的反向代理服务器和缓存服务器，我们在nginx跟node之间加了一层varnish缓存系统，通过配置在varnish缓存整条接口请求，减少相同请求的透传提高中间层服务性能。



中间层：
https://www.cnblogs.com/Renyi-Fan/p/9004177.html


接口聚合： 
https://my.oschina.net/u/4317177/blog/3433497

https://my.oschina.net/u/4317177/blog/3433497


接口性能优化

拆分大接口为独立小接口，并发请求。串行 => 并行，大幅缩短请求时间。

爱奇艺PC Web NodeJS中间层实践
https://cloud.tencent.com/developer/article/1514745
携程
https://cloud.tencent.com/developer/article/1550325



什么是 BFF
BFF，即 Backend For Frontend（服务于前端的后端），也就是服务器设计 API 时会考虑前端的使用，并在服务端直接进行业务逻辑的处理，又称为用户体验适配器。BFF 只是一种逻辑分层，而非一种技术，虽然 BFF 是一个新名词，但它的理念由来已久。

中台



原文地址：https://www.jianshu.com/p/eb1875c62ad3
 