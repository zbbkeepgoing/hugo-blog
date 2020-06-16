---
title: "Hugo Init"
date: 2020-06-15T22:49:20+08:00
draft: false
tags: ["Blog"]
categories: ["Hugo"]
---



### Hugo

##### 安装(windows)

1. 按照[hugo官网](https://gohugo.io/getting-started/installing/#windows)安装即可

2. 验证hugo

   ```sh
   F:\hugo\Sites\zbbkeepgoing\themes>hugo version
   Hugo Static Site Generator v0.72.0-8A7EF3CF windows/amd64 BuildDate: 2020-05-31T
   12:08:42Z		
   ```

##### 创建blog

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
   binbin@binbin-pc MINGW64 /f/hugo/Sites/zbbkeepgoing (master)
   $ ll
   total 28
   drwxr-xr-x 1 binbin 197121     0 六月 15 02:45 archetypes/ 
   -rw-r--r-- 1 binbin 197121 12308 六月 15 09:12 config.toml #hugo配置
   drwxr-xr-x 1 binbin 197121     0 六月 15 10:16 content/    #文章存储位置
   drwxr-xr-x 1 binbin 197121     0 六月 15 02:45 data/          
   drwxr-xr-x 1 binbin 197121     0 六月 15 02:45 layouts/    #全局样式，优先于themes
   drwxr-xr-x 1 binbin 197121     0 八月 30  1754 public/     #编译后出现该目录，blog的静态文件
   drwxr-xr-x 1 binbin 197121     0 六月 15 05:41 resources/     
   drwxr-xr-x 1 binbin 197121     0 六月 15 02:45 static/     #静态文件，优先于themes
   drwxr-xr-x 1 binbin 197121     0 六月 16 02:32 themes/     #主题目录
   ```

#####  创建新文章

1. 创建一篇新文章

   ```
   F:\hugo\Sites\test>hugo new post/myfirst.md
   F:\hugo\Sites\test\content\post\myfirst.md created
   ```

   

2. 

3. 



### md编辑器选择

​		md的编辑器有很多，有在线的、本地的。在这里推荐一款笔者常用的编辑器[typora](https://www.typora.io/)

### Theme内容修改

​		有时候如果我们需要修改Theme中的样式，比如宽度，颜色等等css，我们需要将Theme进行重新编译，才

可以让修改的内容生效。

#### 安装Nodejs & Yarn(Windows)

##### NodeJs安装

1. 下载最新版本Node.js :https://nodejs.org/en/download/

2. 默认一路下一步，即可安装好node,

3. 测试Node.js是否成功: node --version

   ```sh
   F:\>node --version
   v12.18.0
   ```

##### Yarn安装

1. npm安装yarn

   ```sh
   F:\>npm install -g yarn
   C:\Users\binbin\AppData\Roaming\npm\yarnpkg -> C:\Users\binbin\AppData\Roaming\n
   pm\node_modules\yarn\bin\yarn.js
   C:\Users\binbin\AppData\Roaming\npm\yarn -> C:\Users\binbin\AppData\Roaming\npm\
   node_modules\yarn\bin\yarn.js
   + yarn@1.22.4
   added 1 package in 8.561s
   ```

   验证yarn

   ```
   F:\>yarn --version
   1.22.4
   ```

#### 修改theme后编译

​	