[Back](../README.md)

## ruoyi-vue-pro

<hr>

### 1. 简介
>基于 Spring Boot + MyBatis Plus + Vue & Element 实现的后台管理系统 + 微信小程序，支持 RBAC 动态权限、数据权限、SaaS 多租户、Flowable 工作流、三方登录、支付、短信、商城等功能。

#### 仓库位置
- 后端
  mcp-jsw->Server->ruoyi-vue-pro
&nbsp;

- 前端(Vue2 Admin)
  mcp-jsw->Front->yudao-ui-admin  

#### 架构图

![架构图](https://static.iocoder.cn/ruoyi-vue-pro-architecture.png?imageView2/2/format/webp)

&nbsp;

### 2. 开发指南

#### 2-1. 快速启动(后端)

1. 使用IDEA打开{YourWorkFolder}/ruoyi-vue-pro
2. MySQL下创建一个名字为 ruoyi-vue-pro 数据库
3. 导入sql/mysql/ruoyi-vue-pro.sql到ruoyi-vue-pro 数据库
4. application-local.yaml文件中mysql密码改成你本地的
5. 本地启动redis-server(需要版本>=5.0)
6. 启动yudao-server->YudaoServerApplication


<hr>

#### 2-2. 快速启动(前端)

_注意，Node 请使用 14 或者 16 的版本！！！_

```
# 进入项目目录
cd yudao-ui-admin

# 安装 Yarn，提升依赖的安装速度
npm install --global yarn

# 安装依赖
yarn install

# 启动服务()
npm run front
```





