### 必要资源
* github创库，并创建github pages 
    * 最好下载github desktop，然后folk到本地端。
    * github pages 的URL必须是 用户名.github.io （比如我的是github名是：zhihaopy，我的URL就是 zhihaopy.github.io ）
* jekyll环境的搭建：
    * 安装Ruby：[详细步骤可见此](https://hanteng.github.io/notes_tech/jekyll/Ruby/)（由于某些原因，顺利安装是运气，装不到是正常，所以耐着性子，缺啥装啥。也花不了啥时间。）
    * jekyll 是一个简单的博客形态的静态站点生产机器。
    * [jekyll目录结构](http://jekyllcn.com/docs/structure/)（磨刀不误砍柴工，看一下大致了解，好上手）

### 必须了解的
* _config.yml 是配置文件，你可以在里面配置你博客会用到的常量，比如博客名，邮件
* _includes：就是你文章各个部分的html文件，可以在布局中包含这些文件
* _layouts：存放模板。就是你网页的布局，主页布局，文章布局。当然不是指CSS那样的布局，是指，你包含哪些基本的内容到页面上。包含的内容就是includes里面的文件。
* _posts: 存放博客文章
* index：博客主页
* CNAME文件：域名地址
* CSS：存放博客所用CSS
* JS: 存放博客所用JavaScript 

## 具体步骤
### 选择你喜欢的jekyll 主题
* jekyll [themes](http://jekyllthemes.org/)
* 在github搜索 blog/jekyll
* 最好点进去看github主页的 readme.md ，有些博主会介绍其博客的结构或使用说明，选容易的先上手


### _config.yml的更改
* 你可以在里面配置你博客会用到的常量，比如博客名，邮件。（期末项目增加加affiliation 所属单位信息，在你需要显示的地方添加该行
 ：```{{ site.affiliation }}``` [具体操作可见](https://github.com/hanteng/hanteng.github.io/commit/ace637f070c812d7fd11ae25014ed0892aa81b6b)）

### 文章（posts）的写法
```md
---
layout: posttitle: "Welcome to Jekyll!"
date: 2014-01-27 21:57:11
categories: Blog
---
```
* 这一段是必要的，还可以根据个人需要添加如：tags
* 文章放在posts里面
* 文章多用Markdawn语法，可自行百度Markdawn的基本用法，也可用有道云笔记编辑。


### 如何增加多级目录？
* 在文章的开题这段代码中：
```md
layout: post 
title: "弹性布局与响应式图片" 
date: 2017-12-30 22:07:50 
tags: "note_rwd" 
categories:
- posts
- rwd
```





[笔记有参考于](http://www.cnblogs.com/kzd666/p/4733996.html)