


## SetUp
1. 安装RVM `curl -L https://get.rvm.io | bash -s stable`
2. 重新打开终端或者`source ~/.rvm/scripts/rvm`获取RVM环境
3. 检查RVM安装是否正确 `rvm -v`
4. RVM安装Ruby `rvm install 2.6.0`
5. 设置Ruby版本 `rvm 2.6.0 --default`
6. 检查Ruby `ruby -v`
7. 检查gem `gem -v`
8. 替换Ruby源 `gem source -r https://rubygems.org/`
9. 设置为淘宝源 `gem source -a https://ruby.taobao.org`
10. 验证是否替换成功 `gem sources -l`
11. 安装[Jekyll](http://jekyllrb.com) `gem install jekyll`

## Start
1. `git clone https://github.com/xuchuan666/xuchuan666.github.io.git`
2. `bundle install`
3. `bundle exec jekyll serve`
4. open in your browser:`http://localhost:4000`

## Site Settings
```
# Site settings
title:  # 你的博客网站标题
description: # 站点描述
keyword:  # 网站关键词
url:  # 站点url

# Build settings
paginate: 6 # 一页放几篇文章
paginate_path: 'page:num'
```
大部分参数已经默认配置好了，你只需要通过文档了解它们，然后根据自己的需求去`_config.yml`文件里修改即可。

## 写一篇文章
文章一般都放在`_posts`文件夹里，每篇文章的开头都需要设置一些头信息：
```
---
layout: post
title: '标题'
subtitle: '描述'
date: 2017-04-18
categories: 技术
cover: 'http://a.jpg'
tags: 前端开发
---
```
