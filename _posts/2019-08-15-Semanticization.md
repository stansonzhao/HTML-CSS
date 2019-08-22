---
layout: post
title: HTML语义化
date: 2019-08-15 17:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
Hyper Text Markup Language, an application under the standard universal markup language. HTML is not a programming language, but a markup language that is essential for web page creation.

Cascading Style Sheets (English name: Cascading Style Sheets) is a computer language used to represent file styles such as HTML (an application of the standard universal markup language) or XML (a subset of the standard universal markup language).
# 语义化

## 什么是语义化
    1、每一个HTML元素都有具体的含义
    如：
        a元素:超链接
        p元素:段落
        h1元素:一级标题
        ...
    2、所有元素与展示效果无关
        元素展示到页面中的效果，应该由CSS决定
        因为浏览器带有默认的CSS样式，所以每个元素由一些默认样式。

 **总结:选择什么元素，取决于内容的含义，而不是显示出的效果**

## 为什么要语义化？
    1、为了方便搜索引擎优化（SEO）
    常用国内搜索引擎有:百度、搜搜、Bing，国外:Google
    每隔一段时间，搜索引擎会从整个互联网中抓取页面源代码
    
    2、为了让浏览器理解网页
        