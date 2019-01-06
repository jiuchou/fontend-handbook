# 收藏夹图标

所谓favicon，即Favorites Icon的缩写，顾名思义，便是其可以让浏览器的收藏夹中除显示相应的标题外，还以图标的方式区别不同的网站。

## 首页标题前增加小图标显示

### 制作ico文件

1. 在线制作

* [Favicon.ico 在线制作](http://www.faviconico.org/)

  ` 支持.jpg .jpeg .gif .png等图像格式，可在线预览，确认完成再下载`

* [在线制作ico图标](http://www.bitbug.net/)

  `支持.jpg .jpeg .gif .png等图像格式，确认生成文件即下载，无预览功能`

* [在线生成透明ICO图标](http://ico.duduxuexi.com/)

  `支持.png .jpg .gif图像格式，提供`[在线透明圆角工具](http://yj.duduxuexi.com/)`链接地址`


2. 离线制作（暂未提供）

### 基于webpack环境vue组件

想要让favicon.ico 的兼容性更好，favicon.ico图标一般建议放在根目录。放在其他目录，页面加载可能获取不到。 
如果是`vue-cli(脚手架)`搭建的项目，需按以下内容进行修改:

1. 修改配置文件 `build/webpack.dev.conf.js`

```javascript
new HtmlWebpackPlugin({
    filename: 'index.html',
    template: 'index.html',
    inject: true,
    // 增加favicon内容
    favicon: './favicon.ico'
})
```

2. 修改入口文件`index.html`

```html
<link rel="shortcut icon" href="./favicon.ico" type="image/x-icon"/>
```

3. 重新编译运行

```bash
npm run dev
# 或: npm run build
```

