---
published: false
layout: post
title: how_to_use_jekyll
description: ""
category: null
tags: 
  - jekyll
---


## using jekyll build blog##

- 为了在本地可以看到博客的效果，所以要在本地安装jekyll
    1. 直接使用源码安装ruby，安装在$HOME/usr/local/ruby下
    2. 使用gem 安装jekyll。jekyll是ruby库的管理工具，默认安装路径在：???
        
        `gem install jekyll`
    3. 启动jekyll, See it in action at http://localhost:4000.
          
        `jekyll server`

- 根据教程开始建站 http://jekyllbootstrap.com/
    1. git clone https://github.com/plusjade/jekyll-bootstrap.git
    2. jekyll server启动看看效果，个人的blog就是以此为基础开始搭建的

- 个性化定制
    1. _config.yml
        - author,title更改
        - post的url定制
            `permalink: /:categories/:year/:month/:day/:title/` 
        - post 评论设置
        - analytic 
    2. 安装主题
        1. 浏览喜欢的主题 http://themes.jekyllbootstrap.com/preview/hooligan/
        2. 下载/安装 
              `rake theme:install git="https://github.com/dhulihan/hooligan.git"`
        3. 只安装 
              `rake theme:install name="THEME-NAME"`
        4. 只切换
              `rake theme:switch name="the-program"`
- 设计page
    `rake page name="pages/about" `

- 如何发表文章
    1. 使用命令rake post title=""创建一个post
    2. 在_posts/目录下面就可以看到一个文件，使用markdown语法就可以开始blogging啦
