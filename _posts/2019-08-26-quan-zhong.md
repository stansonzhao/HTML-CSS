---
layout: post
title: CSS权重计算
date: 2019-08-24 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 层叠
    解决声明冲突的过程，浏览器自动处理(权重计算)

## 声明冲突
    同一个样式，多次应用到同一个元素

## 1、比较重要性

重要性从高到底:
> 作者样式表:开发者书写的样式表
1、作者样式表中的!important样式，表示这是一个重要样式，重要性最高，权重值为正无穷
2、作者样式表中的普通样式
3、浏览器默认样式表中的样式
## 2、比较特殊性

>看选择器权重
总体规则:选择器权重越大越重要
内联样式权重为1000
ID选择器样式权重为100
类选择器、属性选择器、伪类选择器权重为10
元素选择器、伪元素选择器权重为1

**比较样式选择器权重的时候把该样式所有选择器权重加起来**


## 3、比较源次序

    同样的权重下，代码书写靠后的生效

## 应用

    1、重置样式表
        书写一些作者样式表。覆盖默认样式

a元素伪类书写顺序
    link->visited->hover->active
