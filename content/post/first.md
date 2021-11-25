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
# comment: false # Disable comment if false.
---

本文主要介绍如果通过此平台发布您的文章，顺带对 notice 进行了简单使用
<!--more-->

# 发布你的第一篇文章

创建第一篇文章，放到 post 目录，方便之后生成聚合页面。

```
hugo new post/first.md
```

打开编辑 `post/first.md` ：

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

# 使用 notice
```
{{/% notice note "Note" /%}}
This is a standard "note" style.
{{/% /notice /%}}
```
notice 后面的 参数有四种：note, info, tip 和 warning

{{% notice note "Note" %}}
This is a standard "note" style.
{{% /notice %}}

{{% notice info "Info" %}}
Here is the "info" style.
{{% /notice %}}

{{% notice tip "Tip" %}}
Here is a "tip" variant of a notice.
{{% /notice %}}

{{% notice warning "Warning" %}}
Here is the "warning" flavor of a notice.
{{% /notice %}}

一些更丰富的用法如：

{{% notice tip "Complex Notices are Possible!" %}}
This is a notice that has a lot of various kinds of content in it.  

* Here is a bulleted list
* With more than one bullet 
    * And even more than one level

Code blocks are fine here, too....
```csharp
public void SayHello()
{
    Console.WriteLine("Hello, world!");
}
```
{{% /notice %}}

> 这些 case 都可以通过查看具体代码来找到使用方式