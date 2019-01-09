# 基于vue2+vue-cli3+webpack4构建项目

[使用Vue-Cli3+Webpack4搭建项目](https://segmentfault.com/a/1190000016647573)

vue run serve

项目构建

技术参考点
* [Vue CLI升级](https://cli.vuejs.org/zh/guide/installation.html)
* [快速原型开发](https://cli.vuejs.org/zh/guide/prototyping.html)

操作
npm uninstall vue-cli -g
npm install -g @vue/cli@3.2.1
npm install -g @vue/cli-service-global@3.2.1
`使用vue init, 安装桥接工具`
npm install -g @vue/cli-init@3.2.0
npm install -g webpack@4.26.1

创建并测试项目
1.创建
vue create auth-admin-frontend
或
vue ui
2.运行
npm install --save-dev webpack@4.26.1
npm run serve

创建并测试项目
1. vue init webpack frontend
2. npm install
3. npm run dev



开发配置
1.使用eslint

* [.eslintrc.js模板](https://github.com/PanJiaChen/vue-element-admin/edit/master/.eslintrc.js)

1.1 安装插件

```bash
npm install --save-dev @vue/eslint-config-prettier
```

1.2 配置

根据.eslintrc.js模板内容配置.eslintrc.js文件



前后端交互相关内容

* [请求: GET/POST区别](https://blog.csdn.net/u012391923/article/details/53197387)



项目：
https://github.com/PanJiaChen/vue-element-admin
https://github.com/mgbq/nx-admin
https://github.com/lss5270/vue-admin-spa
https://github.com/beidan/photoShare

文档：
https://github.com/mgbq/nxAdmin-template
https://blog.csdn.net/qq_32340877/article/details/79416344
https://juejin.im/post/591aa14f570c35006961acac
https://juejin.im/post/595b4d776fb9a06bbe7dba56 
https://segmentfault.com/a/1190000009275424#articleHeader8

vue官网：
[Mock.js](http://mockjs.com/)
https://cn.vuejs.org/v2/guide/reactivity.html#%E5%A3%B0%E6%98%8E%E5%93%8D%E5%BA%94%E5%BC%8F%E5%B1%9E%E6%80%A7

rest-framework解释：django token 
https://www.django-rest-framework.org/api-guide/permissions/

归档地址：
https://github.com/Gtry/ManageProject





```
npm install eslint babel-eslint eslint-loader --save-dev

npm install eslint-loader eslint-config-enough --save-dev
```



[Webpack 4 和单页应用入门](https://github.com/wallstreetcn/webpack-and-spa-guide/blob/master/README.md)

1. 使用`vue ui`构建项目
2. 给项目加上语法报错和代码规范检查

```
# 依赖
eslint
babel-eslint
eslint-loader
eslint-config-enough
```

`package.json`增加

```
{
  "eslintConfig": {
    "extends": "enough",
    "env": {
      "browser": true,
      "node": true
    }
  }
}
```

3. 安装 webpack 和 Babel

```bash
webpack
webpack-cli
webpack-serve
html-webpack-plugin
html-loader
css-loader
style-loader
file-loader
url-loader

# babel
@babel/core
@babel/preset-env
babel-loader
```

