# Visual Studio Code

> 笔者机器为Windows系统，本篇内容主要为VSCode在Windows平台中的使用介绍。

Visual Studio Code (简称 VS Code / VSC) 是一款免费开源的现代化轻量级代码编辑器。
软件跨平台支持 Win、Mac 以及 Linux，运行流畅。支持几乎所有主流的开发语言的语法高亮、智能代码补全、自定义快捷键、括号匹配和颜色区分、代码片段、代码对比 Diff、GIT命令 等特性，支持插件扩展，并针对网页开发和云端应用开发做了优化。

## 1 安装

软件下载地址: https://code.visualstudio.com/

下载Visual Studio Code安装包，按照windows系统安装软件方式安装软件即可。

## 2 插件

### 2.1 插件安装

#### 2.1.1 在线安装

#### 2.1.2 离线安装

* 参考
  * [VSCode 插件离线安装](https://blog.csdn.net/wangwei703/article/details/54020712)
  * [简单的 VSCode 插件离线安装方法](https://blog.csdn.net/u012814856/article/details/80684376)

1. 获取插件

插件下载地址: `https://marketplace.visualstudio.com/VSCode`

下载的插件格式后缀为`.vsix`

2. 安装

Window下进入cmd，执行`code --install-extension [test.vsix]`

> 前提： code命令已经添加到环境变量中（code命令路径为VSCode安装路径bin/目录下）

3. 重启VSCode

## 3 常用插件介绍

### 3.1 中英文切换

### 3.2 Vue插件

#### 3.2.1 Vetur

* 参考: [如何优雅地使用 VSCode 来编辑 vue 文件](https://www.clarencep.com/2017/03/18/edit-vue-file-via-vscode)

1. 安装 Vetur 插件

安装方式参考[2.1 插件安装](### 2.1 插件安装)

2. 安装eslint

```cmd
npm install -g eslint
npm install -g eslint-plugin-html
```

3. 配置

```
{
    // 支持vue文件的基本语法高亮
    "emmet.syntaxProfiles": {
        "vue-html": "html",
        "vue": "html"
    },
    // 配置ESLint
    "eslint.validate": [
        "javascript",
        "javascriptreact",
        "html",
        "vue"
    ],
    "eslint.options": {
        "plugins": ["html"]
    }
}
```

### 3.2.2 Eslint

### 3.2.3 Prettier - Code formatter

* [vscode + prettier 专治代码洁癖](https://blog.csdn.net/anxin_wang/article/details/81234214)

1. 安装 Prettier 插件

安装成功后，编辑器默认的格式化处理就会被prettier代替， 默认快捷键是alt + shift + f

2. 配置

## 4 扩展

* [强大的 VS Code](https://www.imooc.com/article/39349)