---
title: "Hugo Init"
date: 2020-06-15T22:49:20+08:00
draft: false
tags: ["Blog"]
categories: ["Hugo"]

weight: 10
contentCopyright: MIT
mathjax: true
autoCollapseToc: true
---



# Hugo

## 安装(windows)

1. 按照[hugo官网](https://gohugo.io/getting-started/installing/#windows)安装即可

2. 验证hugo

   ```
   F:\hugo\Sites>hugo version
   Hugo Static Site Generator v0.72.0-8A7EF3CF windows/amd64 BuildDate: 2020-05-31T
   12:08:42Z		
   ```

## 创建blog

1. 创建一个blog site

   ```
   F:\hugo\Sites>hugo new site zbbkeepgoing
   Congratulations! Your new Hugo site is created in F:\hugo\Sites\zbbkeepgoing.
   
   Just a few more steps and you're ready to go:
   
   1. Download a theme into the same-named folder.
      Choose a theme from https://themes.gohugo.io/ or
      create your own with the "hugo new theme <THEMENAME>" command.
   2. Perhaps you want to add some content. You can add single files
      with "hugo new <SECTIONNAME>\<FILENAME>.<FORMAT>".
   3. Start the built-in live server via "hugo server".
   
   Visit https://gohugo.io/ for quickstart guide and full documentation.
   ```

2. 创建成功后会在目录下面出来一堆文件夹

   ```
   F:\hugo\Sites\zbbkeepgoing>dir
   2020/06/16  12:04    <DIR>          archetypes
   2020/06/16  12:04     82            config.toml   #hugo配置
   2020/06/16  12:04    <DIR>          content       #文章存储位置
   2020/06/16  12:04    <DIR>          data      
   2020/06/16  12:04    <DIR>          layouts       #全局样式，优先于themes
   2020/06/16  12:32    <DIR>          resources
   2020/06/16  12:04    <DIR>          static        #静态文件，优先于themes
   2020/06/16  12:04    <DIR>          themes        #主题目录
   ```

##  创建新文章

1. 创建一篇新文章

   ```
   F:\hugo\Sites\zbbkeepgoing>hugo new post/myfirst.md
   F:\hugo\Sites\zbbkeepgoing\content\post\myfirst.md created
   ```

2. content\post\目录下就会创建出myfirst.md文件

   ```
   F:\hugo\Sites\zbbkeepgoing>cd content
   F:\hugo\Sites\zbbkeepgoing\content>cd post
   F:\hugo\Sites\zbbkeepgoing\content\post>dir
   2020/06/16  12:32     70       myfirst.md
   ```

3. myfirst.md文件内容

   ```
   F:\hugo\Sites\zbbkeepgoing\content\post>type myfirst.md
   ---
   title: "Myfirst"
   date: 2020-06-16T12:32:08+08:00
   draft: true   #代表草稿文件，正式发布前需要修改为false或者删除该字段
   ---
   ```

## 安装主题

​		hugo默认是没有主题的，需要从[hugo主题列表](https://themes.gohugo.io/)或者github中clone一个主题下来。

1. ​	

# md编辑器选择

​		md的编辑器有很多，有在线的、本地的。在这里推荐一款笔者常用的编辑器[typora](https://www.typora.io/)

# Theme内容修改

​		有时候如果我们需要修改Theme中的样式，比如宽度，颜色等等css，我们需要将Theme进行重新编译，才

可以让修改的内容生效。

## 安装Nodejs & Yarn(Windows)

### NodeJs安装

1. 下载最新版本Node.js :https://nodejs.org/en/download/

2. 默认一路下一步，即可安装好node,

3. 测试Node.js是否成功: node --version
 ```
F:\>node --version
v12.18.0
 ```

### Yarn安装

1. npm安装yarn

   ```
   F:\>npm install -g yarn
   C:\Users\binbin\AppData\Roaming\npm\yarnpkg -> C:\Users\binbin\AppData\Roaming\n
   pm\node_modules\yarn\bin\yarn.js
   C:\Users\binbin\AppData\Roaming\npm\yarn -> C:\Users\binbin\AppData\Roaming\npm\
   node_modules\yarn\bin\yarn.js
   + yarn@1.22.4
   added 1 package in 8.561s
   ```

2. 验证yarn

   ```
   F:\>yarn --version
   1.22.4
   ```

## 修改theme后编译

​	