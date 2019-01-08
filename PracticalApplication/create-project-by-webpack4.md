# 基于vue2+vue-cli3+webpack4构建项目

[使用Vue-Cli3+Webpack4搭建项目](https://segmentfault.com/a/1190000016647573)

vue run serve



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

