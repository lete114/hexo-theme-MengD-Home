<h1 align="center"><a href="https://github.com/lete114/hexo-theme-MengD" target="_blank">MengD.(点)</a></h1>

<img src="https://cdn.jsdelivr.net/gh/lete114/CDN2/img/zaxiang/HomePage.png" alt="MengD.(点)">


## 介绍
一个简单的Hexo个人主页设计，能够清晰明了的展现你

Demo：[https://lete114.top](https://lete114.top)

Docs：[https://blog.lete114.top/article/Hexo-MengD.html](https://blog.lete114.top/article/Hexo-MengD.html)

注意：目前已转出，不再使用hexo生成[https://github.com/lete114/HomePage](https://github.com/lete114/HomePage)

## 安装

克隆仓库
``` powershell
git clone https://github.com/lete114/hexo-theme-MengD.git MengD-Home
```

进入`cd MengD-Home`执行下面命令
``` powershell
npm install hexo --save
npm install hexo-deployer-git --save
```

相关命令
``` powershell
hexo server # 本地预览(简写hexo s)
hexo generate # 生成静态文件(简写hexo g)
hexo clean # 清理文件缓存
hexo deploy # 部署(简写hexo d)
```

## 配置

### Hexo配置

``` yml
# https://github.com/lete114/hexo-theme-MengD
# MengD.(点)配置

# 你的域名地址
url: https://lete114.top

# 提交
deploy:
    type: git
    repo:     # 提交的仓库地址
    branch: master
```

### 主题配置

防止爬虫抓取内容限制，如果你想自己修改的话，你可以到`themes\MengD\source`下的`robots.txt`自定义

``` txt
# 允许所有用户代理的浏览器爬虫进行访问（爬取数据）
User-agent: *

# 不允许访问的内容
Disallow: /img/
Disallow: /css/
Disallow: /js/
```

主题`_config.yml`配置

``` yml
# language 语言
language: zh-CN

# name 名称
name: Lete乐特

# 自定义页脚字体颜色
footer_color: '#000 '
footer_a_color: '#000'
# 鼠标移动到超链接上显示的颜色
a_hover: '#e58a8a'
# 自定义名称颜色
name_color: '#80bdab'
#自定义描述字体颜色
desc_color: '#000'

# 自定义背景
# bg_img: url(https://cdn.jsdelivr.net/gh/lete114/CDN2/img/wei_er_li_te/3.jpg)
# bg_img: '#fff'
# bg_img: 'white'
bg_img: url(https://cdn.jsdelivr.net/gh/lete114/CDN2/img/wei_er_li_te/3.jpg)
# 开启主页年份
Copyright: 2019

#关键字
keywords: Lete乐特,Java,JavaWeb,Java常用框架,Spring,SpringBoot,SpringMVC,MyBatis,数据库,MySQL,C#,.NET,开发工具,Git,GitHub,Gitee,(My)Eclipse,IDEA, Hexo,Linux,Maven,前端基础知识,HTML,CSS,JavaScript,jQuery,Ajax,Bootstrap,工具&#x2F;资源,教程,分享,推荐,娱乐,摄影,C#,CMD,Developer,Programmer,Coder


# favicon 图标
favicon: /img/favicon.ico

# avatar 头像
avatar: /img/avatar.png

# site description 网站描述
description: 我相信我可以，但我一直在路上，所以我有无限的可能！！

# 个人描述
desc: 我相信我可以，但我一直在路上，所以我有无限的可能！！<br>人生只有一次，大胆的生活，怎么舒服怎么来！！

# 自定义css js
# 如下
# - https://xxx.com/css/css.css
# - https://xxx.com/js/js.js
# - css/css.css
# - js/js.js
css:
  - https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free/css/all.min.css
  - css/Lete.css
#js:
#  - js/js.js

# 自定义图标
iconfont: https://cdn.jsdelivr.net/gh/sviptzk/StaticFile_HEXO@master/butterfly/css/iconfont.min.css
# 图标大小
font_size: 1.6em
# Icon 图标
links:
  iconfont icon-youxiang: mailto:lete@lete114.top
  iconfont icon-github3: https://github.com/lete114
  iconfont icon-icon_doc_fill: https://blog.lete114.top
  iconfont icon-lianjie: https://blog.lete114.top/link/
  iconfont icon-csdn: https://me.csdn.net/Lott0419
  iconfont icon-zhihu: https://www.zhihu.com/people/lete114


# 音乐
## site=全局加载音乐
## home=只有主页加载音乐
## 404=只有404页面加载音乐
music:
  field: 404
  ### autoplay=自动播放 | loop=循环播放 | controls=显示控件 | muted=静音 | src=音频地址
  ### 不推荐：controls、muted、preload
  ### preload=音频在页面加载时进行加载，并预备播放。如果使用 "autoplay"，则忽略该属性
  property:
    autoplay
    loop
    src="https://656e-env-jxscvzag-1301289878.tcb.qcloud.la/music/zenyang.mp3"

## 404页面
error_404:
  # 多少秒后返回首页
  sec: 30
  # 读秒字体颜色
  text_color: '#e58a8a'
  # 404文字描述
  text: '404！页面君找不到这个网页！！'
  # 自定义背景
  # bg_img: url(https://cdn.jsdelivr.net/gh/lete114/CDN2/img/wei_er_li_te/3.jpg)
  # bg_img: '#fff'
  # bg_img: 'white'
  background: url(https://cdn.jsdelivr.net/gh/lete114/CDN2/img/wei_er_li_te/3.jpg)
  # 鼠标移到返回首页按钮
  # 返回首页边框颜色
  border_color: '#7986cb'
  # 返回首页字体颜色
  font_color: '#80bdab'


# 百度分析
baidu: 05e28fb72axxxxxxf5397bf24543fb1

# ICP备案
ICP:
  enable: true
  icon: img/icp.png
  url: http://www.beian.miit.gov.cn/
  text:
```

