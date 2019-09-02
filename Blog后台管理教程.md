# 博客后台管理教程Hexo Admin

教程地址：https://www.cnblogs.com/xingyunblog/p/8681205.html

## hexo Admin 地址 
Hexo Admin 插件GitHub 首页：https://github.com/jaredly/hexo-admin

演示Demo:https://jaredforsyth.com/hexo-admin/
## 1、安装Hexo Admin插件

## Install the admin & start things up

```
npm install --save hexo-admin
hexo server -d
open http://localhost:4000/admin/
```

## 2、Hexo Admin配置登录账号和密码

```
http://127.0.0.1:4000/admin/
```

Tips: 要注意我们只能在本地进行后台管理，无法在自己的域名下进行后台管理

打开之后我们可以看到后台管理界面

![](https://github.com/Soros1990/markDownImages/blob/master/201909021627.png?raw=true)

# ## 执行三道命令，重启我们的博客服务器

清理项目

```
hexo clean
```

 重新构建项目

```
hexo generate
```

启动server

```
hexo server -d
```

 Tips: 如果需要提交代码改动到GitHub上，请在构建项目命令后执行以下命令

```
hexo deploy
```

当我们打开以下网址时候你会发现

```
http://127.0.0.1:4000/admin
```