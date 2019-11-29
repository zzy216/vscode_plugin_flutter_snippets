# vscode插件开发、发布主要流程

[官网](https://marketplace.visualstudio.com/manage)

插件开发前的准备：vscode、nodejs、vscode插件生产工具、git、微软账号
插件开发：插件构思、官方文档查阅
插件发布：打包、上传、插件市场操作
插件维护：更新迭代后打包、上传、插件市场操作 

## 插件开发前的准备：

vscode插件生产工具：官方推荐使用Yeoman 和 VS Code Extension Generator。用如下命令安装：

    npm install -g yo generator-code

### 插件开发

使用生产工具初始化代码

    yo code

在os系统上通过上下键来选择要创建的类型，在win上输入1、2、3后按回车来选择。

### 插件发布
安装打包、发布工具

    npm install -g vsce

### 打包
执行如下命令：

    vsce package

### 发布
方法一：用vsce的vsce publish工具来发布，但是需要在官网配置Personal Access Token较为繁琐。可参考官方教程
https://yanyunianhua.visualstudio.com/_usersSettings/tokens

方法二：在官网直接上传发布https://marketplace.visualstudio.com/