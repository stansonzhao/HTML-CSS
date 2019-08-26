---
layout: post
title: CSS盒模型应用
date: 2019-08-30 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 盒模型应用

## 改变宽高范围

    默认情况下，width和height 设置的是内容盒宽高

> 页面重构师: 将设计稿制作为静态页面

    衡量设计稿尺寸的时候，往往使用的是边框盒，但设置width和height，则设置的是内容盒

        1、精确计算

        2、CSS3: box-sizing:content-box(内容盒),padding-box(填充盒),border-box(边框盒)

## 改变背景覆盖范围

    默认情况下，背景覆盖边框盒

    可以通过background-clip进行修改

## 溢出处理

    宽高定死情况下，文字太多会溢出容器

    overflow，控制内容溢出边框盒后的处理方式 overflow:hidden(隐藏)，visible(可见的)，scroll速写属性(生成滚动条)，overflow-y:scroll，添加滚动条后宽度足够时，滚动条仍在。overflow-y:auto,意思是自动决定是否生成滚动条，高度足够时不出现，不够时自动出现

## 断词规则

    word-break，影响文字在什么位置被截断换行

    normal：普通。 CJK字符(c中国J日本K韩国)(文字位置截断)，非CJK字符(单词位置截断)

    word-break:break-all 截断所有   keep-all在单词之间

## 空白处理

    white-space:nowrap  禁止换行
    overflow:hidden  溢出隐藏
    text-overflow:ellipsis 文字打点