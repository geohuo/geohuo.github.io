---
layout: post
title: 如何在windows平台上基于github搭建个人博客平台
categories: Blog
description: 从零开始学习和搭建个人博客平台
keywords: github，博客搭建，github.io
---

## Github.io 简介

作为一个非前端和网站开发人员，想要自己搭建个人博客来分享日常的学习和生活，一直找了好久的平台。之前在CSDN上写过一些博客，但是许久不更新就懒得再管了。最近因为研究需要，发现有太多的东西需要记录，同时，Markdown也越用越顺手，就想着能够建立自己的博客平台来分享自己平时研究和学习过程中的一些技术问题和自己对于研究的一些思考。后来发现Github提供了这样的平台（原谅我的后知后觉），就想着能够自己搭建一个博客平台。

本人要求不高，主题简洁大方，能够开开心心的分享自己的博文就可以。而github提供的github pages基本上能满足我的需求了，使用也方便，搭建好环境以后，可以使用Markdown来编写博客，并且上传到github上托管，非常方便。

## 一. Markdown 简介

### 1. 语法简介

待完成

### 2. Markdown编辑器typora

为了方便写Markdown，我们需要一个Markdown的解释器来实时预览写出来的效果。市面上有很多支持Markdown语法的代码编辑器可选，例如vscode，sublime text，atom等等。我选择的是一款目前还处于beta阶段的Markdown编辑器[typora](https://www.typora.io)，与传统的分两栏写markdown和预览markdown文件不同的是，typora能够“所见即所得”，写完了就可以实时在当前位置看到最终效果。而且typora本身支持内嵌LaTex数学公式，本人试过，几乎所有的公式都可以嵌入，而且支持公式的自动编号，可以作为平时快速写作的一个高效编辑器。这里不仔细讲typora的用法，网上可以找到许多教程，例如[Typora完全使用详解](https://sspai.com/post/54912)，有兴趣的朋友可以了解一下。

## 二. 搭建过程

### 1. 申请github账号和创建repo

待完成

### 2. 选择自己喜欢的主题

待完成

```
git clone 
```



### 3. 基于ruby的本地编写和调试博客内容

[ruby的下载地址](https://rubyinstaller.org/downloads/)

ruby的安装路径最好不要包含空格（没有完整去验证过，但是我第一次的安装路径包含了空格，后面安装其他东西的时候老是不成功。重新选择了不包含空格的安装路径来安装了ruby后，安装后续的其他问题一路顺利。）

ruby安装完成以后会弹出一个窗口让你选择3个选项之一来安装，一般直接选3就是，安装过程需要一定的时间。如果这部分没有安装成功，可以使用如下的命令重新安装，这个命令直接在windows的cmd中执行即可，后面的其他安装命令也是一样的。安装成功以后直接回车即可。

```shell
ridk install
```


待完成
```shell
gem install bundle
```
待完成

```
gem install jekyll
```

最后需要安装github-pages，这部分会持续安装很多东西，所以耗时比较长，耐心等待即可。
```
gem install github-pages
```

<center>
    <img src="/images/posts/blog/blog-build-blog.png" alt="picture not found" style="zoom:100%;" />
    <br>
</center>

至此，所有的安装工作已完成，你会看到如下界面：



此时cd到对应的目录，运行如下命令：

```
bundle exec jekyll server --watch
```

正常情况下你能看到类似下图的启动界面了，此时在浏览器的地址栏输出 `localhost:4000`就能看到你的博客了。如果不行，请参考后文的常见问题和解决办法。



## 三. 常见问题

### 1. 无法正常安装github-pages...

待完成

### 2. 无法启动jekyll server

待完成



## 四. 参考

1. 非常感谢xxx，本博客的搭建过程使用了xxx的主题