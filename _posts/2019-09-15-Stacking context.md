---
layout: post
title: CSS堆叠上下文
date: 2019-09-15 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 堆叠上下文

    堆叠上下文(stack context)，它是一块区域，这块区域由某个元素创建，它规定了该区域中的内容，在z轴上排列的先后顺序。

## 创建堆叠上下文元素
    1、html元素(根元素)
    2、设置了z-index(非auto)数值的定位元素

## 同一个堆叠上下文的元素在Z轴上的排列

    从后到前的排列顺序：

    1、创建堆叠上下文的元素的背景和边框

    2、堆叠级别(z-index,stack level)为负数的堆叠上下文 z-index值越大靠前，越小靠后，相同值的按书写顺序靠后的在前展示

    3、常规流非定位的块盒

    4、非定位的浮动盒子

    5、常规流非定位行盒

    6、任何z-index是auto的定位子元素，以及z-index是0的堆叠上下文

    7、堆叠级别为正值的堆叠上下文

    每个堆叠上下文，独立于其他堆叠上下文，它们之间不能相互穿插