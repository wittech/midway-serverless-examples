## 如何进行开发？

### 本地开发

```shell
# 首先需要安装开发依赖

$ npm i --registry=https://registry.npm.taobao.org
```

```shell
# 启动 react 本地 watch 和 函数本地 Dev Server
# 在终端中会输出 本地 Dev Server 的URL链接

$ npm run dev
```

> Tips: 可执行 `npm run local:url` 单独获取本地Dev Server 的URL链接

### 配置数据库

默认为读取环境变量，亦可手动在 `config/config.default.ts` 文件内进行修改

| 环境变量名 | 释义 |
| --- | --- |
| MIDWAY_RDS_HOST | RDS 数据库地址 |
| MIDWAY_RDS_PORT | RDS 数据库端口，默认为3306 |
| MIDWAY_RDS_DBNAME | RDS 数据库名称 |
| MIDWAY_RDS_USERNAME | RDS 数据库用户名 |
| MIDWAY_RDS_PASSWORD | RDS 数据库密码 |

### 发布
```shell
# 发布前需要构建前端代码
$ f deploy
```

## About Midway FaaS

Midway FaaS 是用于构建云函数的 Serverless 框架。帮助您在云原生时代大幅降低维护成本，更专注于产品研发。<br />

- **跨云厂商：**一份代码可在多个云平台间快速部署，不用担心你的产品会被云厂商所绑定。
- **代码复用：**通过框架的依赖注入能力，让每一部分逻辑单元都天然可复用，可以快速方便地组合以生成复杂的应用。
- **传统迁移：**通过框架的运行时扩展能力，让 Egg.js 、Koa、Express.js 等传统应用无缝迁移至各云厂商的云函数。


<br />Midway FaaS 是阿里巴巴集团发起的开源项目，由一个专业的 Node.js 架构团队进行维护。已大规模应用于阿里集团各 BU 线上业务，稳定承载了数千万的流量。

查阅[详细文档](https://www.yuque.com/midwayjs/faas/quick_start)
