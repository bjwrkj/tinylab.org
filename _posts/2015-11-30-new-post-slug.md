---
layout: post
author: 'Wu Zhangjin'
title: "new post"
album: "Linux 稳定性优化"
group: original
permalink: /new-post-slug/
description: " 文章摘要 "
category:
  - category1
  - category2
tags:
  - tag1
  - tag2
---

> By Falcon of TinyLab.org
> 2015-11-30

本模板为 泰晓科技 采用的文档模板与约定，为规范文章风格与质量，请在撰稿前务必仔细阅读！

这里分别就几个方面展开介绍：

## 文章分类

为了更好地展示和组织文章，请尽量采用 `_data/categories.yml` 中的分类，如果确实有新增，请在发文前单独提交 PR 更新该文件。

## 内容列表

1. 数字列表，条目 1
  * 普通列表，条目 1
  * 普通列表，条目 2

2. 数字列表，条目 2

## 代码缩进

代码在正文下，用 4 个空格缩进：

    #include <stdio.h>

    int main(void)
    {
       printf('Hello, World!');
    }

*注*: 如果要跟列表一起缩进显示，得添加相应空格。

## 正文内内嵌代码

如果正文中包含了命令、接口、代码片段、变量等属于代码的部分时，请用 ` 括起来，例如：`grep Free /proc/meminfo`，用法为：

    `grep Free /proc/meminfo`

## 中英文以及数字混排

当中 English 文以及中文、数字混排时，记得在 English 和数字，例如 1 2 3 4 周边添加空格，进而确保可阅读性，即 Readability。

## 表格用法

| 标题 1      | 标题 2     | 标题 3          |
|-------------|-----------:|:---------------:|
| 左对齐      |右对齐      | 居中对齐        |

## 在正文中嵌入图片

Markdown 基本语法如下：

![图片名](/images/weibo/tinylaborg.jpg '图片内容提示，可选')

*注*：如果想规范图片大小，想增加额外的特性，可以用 html 的 `<img>` 标记。

## 链接以及各类内容混排

### 链接

* [链接用法一][1]

  在列表后面放入脚本，为了确保跟列表一起缩进，需要额外增加两个空格：

      #!/bin/bash
      echo 'Hello, World.'


* [另外一种链接用法](http://tinylab.org)

  在列表后面再嵌入子列表，包括数字列表和非数字列表：

  * Another list
    * Another list
      1. Third list
      2. Third list


* 第三种链接用法：<http://tinylab.org>

### 更复杂的列表用法

1. 表项 1

    这里再嵌入代码：

        #include <stdio.h>

        int main() { return 0; }

2. 表项 2

    这里嵌入图片：

    ![图片名](/images/weibo/tinylaborg.jpg '图片内容描述信息')

3. 表项 3

    普通正文

4. 表项 4
  * 数字表项嵌入非数字表项，表项 1
  * 表项 2

        | 标题 1      | 标题 2     | 标题 3          |
        |-------------|-----------:|:---------------:|
        | 左对齐      |右对齐      | 居中对齐        |

*注*：数字列表跟普通列表有一个差别是，数字列表后面如果要加正文自动缩进，得增加 4 个空格，而普通列表只需要两个。估计是 Markdown 解释器的问题，请尽量遵循这个约定吧。

## 正文引用

如果要引用第三方的信息，可以这么做：

> 这里是来自第三方的信息，信息内容可以用普通的 Markdown 语法来标记[链接][1]、**加粗**、`命令`等等，很灵活。。。

[1]: http://tinylab.org