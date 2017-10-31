# egg-note
## egg.js 是基于KOA的企业级框架
### 1. eggjs创建项目
使用脚手架：
- $ npm i egg-init -g
- $ egg-init egg-example --type=simple
- $ cd egg-example
- $ npm i
- $ npm run dev  //启动项目
### 2.eggjs的目录结构
- app/router.js 用于编写路由规则（必须）
- app/controller 用于处理用户输入（必须）
- app/public 用于存放静态资源
- app/middleware 用于编写中间件
-- 其余结构用到再说
### router.js
- app.get(url,controller)  controller：可以写成  "home.index" 或 app.controller.home.index
- app.redirect(url,anotherUrl)  重定向 可连接静态资源