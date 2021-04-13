
<!-- 
问题： 使用wifi、网线安装包时经常运行不起来,使用手机共享解决
 -->


### 创建项目

<!-- 
官方安方式
npm init egg --type=simple
npm i
 -->

```bash
# 创建项目 

# egg-init地址： https://github.com/eggjs/egg-init/blob/master/README.zh-CN.md

npm i egg-init -g 

egg-init egg-server --type=simple 

cd egg-server npm i

# 启动项目 
# npm start 和 npm stop 配合使用

npm run dev 

open localhost:7001
```

### 基于插件的Swagger-doc接口定义(接口文档)

```bash
# 插件安装
npm install egg-swagger-doc-feat -s

open localhost:7001/swagger-ui.html
```

### 统一异常处理
### 基于扩展的helper响应统一处理 
### Validate接口格式检查 

### 跨域处理
```bash
# 插件安装
npm install egg-cros -s
```

修改配置

```js
// config/plugin.js
cors:{
    enable: true,
    package: 'egg-cors',
}

// config/config.defaule.js
config.cors = {
    origin: '*',
    allowMethods: 'GET,HEAD,PUT,POST,DELETE,PATCH'
}
```




### 三层结构 
### jwt统一鉴权 
### 文件上传