# fatty

Hexo主题fatty, 基于[writing](https://github.com/yunlzheng/hexo-themes)主题

## Demo

![screenshot](https://raw.github.com/sumory/hexo-theme-fatty/master/source/css/img/demo.png)


## Install

Download the zip file, unzip it and modify `theme` in `_config.yml` to `fatty`.


## Config

``` yaml
menu:
  博客: /
  存档: /archives
  项目: /projects #需自己建立页面，hexo new page projects
  关于: /about

widgets:
- search
- recent_posts
- category
- tag


excerpt_link: Read More

addthis:
  enable: true

fancybox: true

google_analytics:
rss:

comment_provider: duoshuo


# Duoshuo comment
duoshuo:
  short_name: sumory # use your own name

society:
  enable: true
  github: https://github.com/sumory
  weibo: http://weibo.com/***

#About Page
about:
  name:
```

- **menu** - 导航菜单项
- **widget** - 侧边栏工具
- **excerpt_link** - "Read More" link text at the bottom of excerpted articles
- **addthis** - 加网分享按钮
  - **enable** - 是否启用加网分享
- **fancybox** - Enable [Fancybox]
- **google_analytics** - Google Analytics ID
- **rss** - RSS subscription link (change if using Feedburner)
- **duoshuo**: 国内还是用多说来的比较稳定
- **short_name**: 在多说注册的short_name 
