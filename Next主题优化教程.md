# 博客主题优化Next
Next主题

Hexo博客支持很多主题风格，其中Next主题是Github上Star最多的主题，其一直在更新维护，支持非常多的外部插件和功能选项。我目前使用的是Next6.0版本，下面我会介绍基于Next6主题的界面美化手法。

## 1、 Next主题的安装配置

Next主题的安装方式很简单，只需要在博客主目录下执行：

git clone https://github.com/theme-next/hexo-theme-next themes/next

然后设置站点配置文件_config.yml：

theme: next
即可将我们的Hexo博客主题替换为Next主题。

在blog config中添加配置

```
# Extensions
## Plugins: https://hexo.io/plugins/
## Themes: https://hexo.io/themes/
theme: next
```

## 2、Next主题个性化配置

修改Next相关配置均在`themes/next/_config.yml`中修改

###  2.1、修改布局风格

Next默认风格是Muse，可修改为其他

```
# Schemes
# scheme: Muse
scheme: Mist
#scheme: Pisces
#scheme: Gemini
```

### 2.2、修改菜单目录

Next主题默认只有主页和和关于，如果要增加菜单

```
# Usage: `Key: /link/ || icon`
# Key is the name of menu item. If the translation for this item is available, the translated text will be loaded, otherwise the Key name will be used. Key is case-senstive.
# Value before `||` delimiter is the target link.
# Value after `||` delimiter is the name of Font Awesome icon. If icon (with or without delimiter) is not specified, question icon will be loaded.
# When running the site in a subdirectory (e.g. domain.tld/blog), remove the leading slash from link value (/archives -> archives).
# External url should start with http:// or https://
menu:
  home: / || home #主页
  tags: /tags/ || tags #标签
  categories: /categories/ || th #分类
  archives: /archives/ || archive #归档
  about: /about/ || user #关于
  guestbook: /guestbook/ || comment #留言
  #schedule: /schedule/ || calendar
  #sitemap: /sitemap.xml || sitemap
  #commonweal: /404/ || heartbeat
```

### 2.3、添加头像图片

在`themes/next/_config.yml`中修改配置

```
# Sidebar Avatar
avatar: 
  # In theme directory (source/images): /images/avatar.gif
  # In site directory (source/uploads): /uploads/avatar.gif
  # You can also use other linking images.
  url: #/images/avatar.gif
  # If true, the avatar would be dispalyed in circle.
  rounded: false
  # If true, the avatar would be rotated with the cursor.
  rotated: false
```

### 2.4、添加社交账号

```
# Social Links
# Usage: `Key: permalink || icon`
# Key is the link label showing to end users.
# Value before `||` delimiter is the target permalink.
# Value after `||` delimiter is the name of Font Awesome icon. If icon (with or without delimiter) is not specified, globe icon will be loaded.
social:
  GitHub: https://github.com/Soros1990 || github
  E-Mail: mailto:751438921@qq.com || envelope
  #Weibo: https://weibo.com/yourname || weibo
  #Google: https://plus.google.com/yourname || google
  #Twitter: https://twitter.com/yourname || twitter
  #FB Page: https://www.facebook.com/yourname || facebook
  #VK Group: https://vk.com/yourname || vk
  #StackOverflow: https://stackoverflow.com/yourname || stack-overflow
  #YouTube: https://youtube.com/yourname || youtube
  #Instagram: https://instagram.com/yourname || instagram
  #Skype: skype:yourname?call|chat || skype
```

### 2.5、添加站内搜索

安装插件：

```
npm install hexo-generator-search --save
```

修改配置

```
# Local Search
# Dependencies: https://github.com/wzpan/hexo-generator-search
local_search:
  enable: true
  # If auto, trigger search by changing input.
  # If manual, trigger search by pressing enter key or search button.
  trigger: auto
  # Show top n results per article, show all results by setting to -1
  top_n_per_article: 1
  # Unescape html strings to the readable one.
  unescape: false
  # Preload the search data when the page loads.
  preload: false
```

