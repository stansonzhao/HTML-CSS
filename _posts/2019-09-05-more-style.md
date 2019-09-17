---
layout: post
title: CSS更多样式
date: 2019-09-05 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 更多的样式

## 透明度
    1、opacity，设置整个元素的透明度,它的取值是0~1，给盒子设置透明度后，整个盒子和子元素都透明
    2、在颜色位置设置alpha通道，rgba

## 鼠标
    使用cursor设置,可以引入自定义图标作为cursor
    cursor:url(),auto;auto是为了兼容性

## 盒子隐藏
    1、display:none;表示不生成盒子，可能会影响其它盒子排班
    2、visibility:hidden,生成盒子，只是从视觉上移除盒子，盒子仍然占据空间。值有visibility（显示）,hidden（隐藏）。

## 背景图
    background-image

### 和img元素的区别
    img元素属于HTML的概念


    背景图属于CSS的概念
    
    1、当图片属于网页内容时，必须使用img元素
    2、当图片仅用于网页的美化时，必须使用背景图

### 涉及的CSS属性

    1、background-image 
        url()....

    2、background-repeat 值有no-repeat,repeat-x,repeat-y

        默认情况下，背景图会在横坐标和纵坐标中进行重复

    3、background-size
        预设值contain、cover，类似于object-fit
        数值或百分比，横向和纵向，

    4、background-position
        设置背景图位置
        预设值center(横向纵向居中)，left(靠左),right(靠右)，top(靠上)，bottom(靠下)。可以组合如center top，center bottom等等
        数值或百分比,第一个值代表离左边距离，第二个值代表离上边距离
        雪碧图(精灵图)(spirit)

    5、background-attachment
        设置背景图相对视口是否固定
        预设值：fixed
    
    6、背景图和背景颜色混用
        background-image
        background-color
        当背景图无法完全覆盖盒子时，可以利用与图片边缘色相近的颜色做背景色来代替图片覆盖

    7、速写属性 background
        background:imageURL no-repaet position/size color attachment
        