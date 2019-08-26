---
layout: post
title: HTML之文本元素
date: 2019-08-15 18:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---

# 文本元素
HTML5中支持的元素：HTML5元素周期表

## h[1~6]
    h1~h6 表示一级标题到六级标题

## p
    p:段落标签，paragraphs(段落)
    生成随机文字可用Lorem，乱数假文，没有任何实际含义的文字。lorem后可以加数字，代表生成多少个单词

## span
    span:无语义，仅用于设置样式
    以前某些元素在显示时会独占一行(块级元素)，而某些元素不会(行级元素)
    HTML5中块级相当于流内容类别，行级相当于措辞内容类别
    
## pre
    pre:预格式化文本元素
    空白折叠:在源代码中的连续空白字符(空格、换行、制表)，在页面显示时，会被折叠为一个空格
    例外:在pre元素中的内容不会出现空白折叠
    在pre元素内部出现的内容，会按照源代码格式显示在页面上。
    显示代码时，通常外面套code元素，code表示代码区域。