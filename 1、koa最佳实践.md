### 创建项目

```bash
mkdir koa-project
cd koa-project
npm init -y

npm i koa -S
```

### 搭建koa服务

```bash
const koa = require("koa");
const app = new koa();

app.use(async ctx => {
    console.log("hello koa");
});

app.listen(7000);

```
### 插件安装

``` bash
npm i koa-router koa-static koa-bodyparser multer mysql -S
```

|  插件               | 注解  |
|  ----              | ----  |
| koa-router         | 路由管理中间件 |
| koa-static         | 静态资源中间件 |
| koa-bodyparser     | 解析请求内容 |
| multer             | 用于处理 multipart/form-data 类型的表单数据，它主要用于上传文件 |
| busboy             | 用来解析POST请求，node原生req中的文件流。 |
| mysql              | 数据库 |
| koa-logger         | 日志 |



### 项目结构
```
├── init # 数据库初始化目录
│   ├── index.js # 初始化入口文件
│   ├── sql/    # sql脚本文件目录
│   └── util/   # 工具操作目录
├── config  # 配置文件
│   ├── config.js # 
├── server  # 后端代码目录
│   ├── app.js # 后端服务入口文件
│   ├── routers/ # 路由目录
│   ├── controllers/    # 操作层目录
│   ├── services/   # 业务层目录
│   ├── models/ # 数据模型model层目录
│   ├── utils/  # 工具类目录
│   └── views/  # 模板目录
├── static # 前端静态代码目录
│   ├── build/   # webpack编译配置目录
│   ├── output/  # 编译后前端代码目录&静态资源前端访问目录
│   └── src/ # 前
│
└── package.json 

```




### 参考

[《Koa2进阶学习笔记》已完结](https://chenshenhai.com/koa2-note)

[大深海github地址](https://github.com/chenshenhai/koa2-note/blob/master/note/start/quick.md)

[《koa2中文文档》](https://www.itying.com/koa/article-index-id-83.html)