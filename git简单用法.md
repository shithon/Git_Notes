---
title: “简单操作github”
tags: tech
author: Wang xu
top: False
---

### github

最近在把自己写的代码和东西倒腾到github上去，因为之前有写前端以及git的一些知识，所以这里只是简单的总结了下：

#### Git操作

##### 本地操作：
A、先建个文件
--cd /d/Devp/Project
--mkdir Resume
--cd Resume
--git init     *初始化一个目录*
--touch index.html
--mkdir css js
--touch css/style.css js/main.js

B、初始化一个项目过后就可以开始在本地操作了

1、首先git add 可以一个一个add 也可以全部add
git add index.html
git add css/style.css
git add js/main.js
或者git add .（.号前面一定要空格）

2、git commit -m
a.	git commit index.html -m '添加index.html'
b.	git commit css/style.css -m "添加 css/style.css"
或者一次性添加
git commit . -m"添加了几个文件"

3、改动
改动完之后继续 git add .以及 git commit . -m"更新"
4、查看历史 git log

##### 将本地仓库上传至Github
1、在 GitHub 上新建一个空仓库，名字一致
2、点击SSH
3、按照命令一行一行执行即可
【提示你已有一个仓库后面该怎么做…or push an existing repository from the command line
git remote add origin git@github.com:shithon/resume.git
git branch -M main
git push -u origin main

##### 如果后面在本地进行修改完之后怎么上传更新呢？
git进去修改、创建都行
之后先保存到本地 git add 然后 git commit 然后 git pull 最后git push
例子：
1.	cd git-demo-1
2.	touch index2.html
3.	git add index2.html
4.	git commit -m "新建 index2.html"
5.	git pull
6.	git push

#### 把别人的仓库下载到本地
进入一个目录，git clone以git@github.com开头的地址，然后会发现下载好了，可以在别人的目录下进行修改。然后 add commit 再pull push.

by Wang xu in NUS campus