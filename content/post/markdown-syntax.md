+++
author = "glmapper"
title = "语法指导"
date = "2019-03-11"
description = "示例文章展示了 HTML 元素的基本 Markdown 语法和格式。"
featured = true
tags = [
    "markdown",
    "css",
    "html",
    "themes",
    "featured"
]
categories = [
    "themes",
    "syntax",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
thumbnail = "images/building.png"
+++


本文提供了一个可在 Hugo 内容文件中使用的基本 Markdown 语法示例，还展示了基本 HTML 元素是否在 Hugo 主题中使用 CSS 装饰。
<!--more-->

## Headings

以下 HTML `<h1>`—`<h6>` 元素代表六级节标题。 `<h1>` 是最高的部分级别，而 `<h6>` 是最低的。

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Blockquotes

blockquote 元素表示从另一个来源引用的内容，可以选择带有必须在 `footer` 或 `cite` 元素内的引文，并且可以选择带有行内更改，例如注释和缩写。

#### 没有参数的块

> 这是一个非常普通的块段落

> 使用 **加粗** 和 *斜体* .

#### 带有参数的块

> 这是一段引用，并且备注了作者.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## 表格

表格不是核心 Markdown 规范的一部分，但 Hugo 支持开箱即用。

   Name | Age
--------|------
    Bob | 27
  Alice | 23

#### 表格内的内联

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

## 代码块

#### Code block with backticks（反引号）

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
<!-- this line is extraneous 2Error from server (Forbidden): deployments.apps is forbidden: User "chiptest" cannot create resource "deployments" in API group "apps" in the namespace "default" -->
</html>
```

#### 四个空格缩进的代码块

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### 带有 Hugo 内部高亮短代码的代码块
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## 列表类型

#### 排序列表

1. First item
2. Second item
3. Third item

#### 无序列表

* List item
* Another item
* And another item

#### 多级列表

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## 其他元素 — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.
