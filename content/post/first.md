---
title: "快速开始" # Title of the blog post.
date: 2021-11-25T09:50:49+08:00 # Date of post creation.
description: "如何通过 hugo 发布你的文章" # Description used for search engine.
featured: true # Sets if post is a featured post, making appear on the home page side bar.
draft: false # Sets whether to render this page. Draft of true will not be rendered.
toc: true # Controls if a table of contents should be generated for first-level links automatically.
author: "glmapper"
# menu: main
#featureImage: "/images/path/file.jpg" # Sets featured image on blog post.
#humbnail: "/images/path/thumbnail.png" # Sets thumbnail image appearing inside card on homepage.
shareImage: "/images/path/share.png" # Designate a separate image for social media sharing.
codeMaxLines: 10 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: false # Override global value for showing of line numbers within code block.
figurePositionShow: true # Override global value for showing the figure label.
categories:
  - Technology
tags:
  - test
---

本文主要介绍如何通过此平台发布您的文章，对于如何使用 hugo 不做过多说明。

<!--more-->

{{% notice info "特别申明" %}}
本技术博客平台基于 [hugo](https://gohugo.io/), 使用了[clarity](https://github.com/chipzoller/hugo-clarity) 作为默认主题，在此对参与上述项目的所有社区贡献者表示感谢！
{{% /notice %}}

# 本地运行

1、从 github 上 clone 项目工程

> git clone https://github.com/huami-tech/huami-tech.github.io.git

2、cd 到工程目录下

3、执行 `hugo server` 

4、浏览器打开 localhost:1313 即可浏览

# 发布你的第一篇文章

1、从 github 上 clone 项目工程

> git clone https://github.com/huami-tech/huami-tech.github.io.git

2、cd 到工程目录下，创建第一篇文章（放到 post 目录，方便之后生成聚合页面），如文件名为 first.md

```
hugo new post/first.md
```

3、打开编辑 `post/first.md` ：

```
---
date: "2015-10-25T08:36:54-07:00"
title: "first"
 
---
### Hello Hugo
 1. aaa
 1. bbb
 1. ccc
```

4、提交代码即可

