---
layout: post
title: HTML之元素包含关系
date: 2019-08-21 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
Hyper Text Markup Language, an application under the standard universal markup language. HTML is not a programming language, but a markup language that is essential for web page creation.

Cascading Style Sheets (English name: Cascading Style Sheets) is a computer language used to represent file styles such as HTML (an application of the standard universal markup language) or XML (a subset of the standard universal markup language).
# 元素包含关系
    以前:块级元素可以包含行级元素，行级元素不可以包含块级元素，a元素除外

    现在:元素的包含关系由元素的内容类别决定。
    
    例如，查看h1元素中是否可以包含p元素 (可在MDN查询)
## 总结
    1、容器元素中可以包含任何元素
    2、a元素中几乎可以包含任何元素
    3、某些元素有固定的子元素(ul>li,ol>li,dl>dt+dd)
    4、标题元素和段落元素不能相互嵌套，并且不能包含容器元素
    