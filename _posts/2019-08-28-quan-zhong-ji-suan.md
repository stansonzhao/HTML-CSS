---
layout: post
title: CSS权重计算
date: 2019-08-28 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 属性值的计算过程
    渲染每个元素的前提条件:该元素的所有CSS属性必须有值
    一个元素，从所有属性都没有值，到所有的属性都有值，这个计算过程，叫做属性值的计算过程
## 属性值计算过程

## 1、确定声明值:参考样式表中没有冲突的声明，作为CSS属性值

![](/assets/img/arrt/1.png)

## 2、层叠冲突:对样式表有冲突的声明使用层叠规则，确定CSS属性值

![](/assets/img/arrt/2.png)

## 3、使用继承:对仍然没有值的属性，诺可以继承，则继承父元素的值

![](/assets/img/arrt/3.png)

## 4、使用默认值:对仍然没有值的属性，使用默认值

![](/assets/img/arrt/4.png)

## 特殊的两个CSS取值
    inherit 强制继承父元素的值 
    initial 初始值，将该属性设为默认值
