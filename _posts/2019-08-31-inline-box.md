---
layout: post
title: CSS的行盒
date: 2019-08-31 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 行盒的盒模型

常见的行盒:包含具体内容的元素

span、strong、em、i、img、video、audio

## 显著特点
    1、盒子沿着内容沿伸，
    2、行盒不能设置宽高

    调整行盒宽高，应该使用字体大小，行高，字体类型，简介调整

    3、内边距(填充区)
    水平方向有效，垂直方向仅会影响背景，不会占据实际空间

    4、边框

    水平方向有效，垂直方向不会占据实际空间

    5、外边距

    水平方向有效，垂直方向不会占据实际空间

## 行块盒
    display:inline-block

    1、不独占一行
    2、盒模型中所有尺寸都有效

## 空白折叠
    发生在行盒(行块盒)内部或行盒(行块盒)之间

## 可替换元素和非可替换元素
    大部分元素，页面显示结果，取决于元素内容，叫**非可替换元素**
    少部分元素，页面显示结果，取决于元素属性，叫**可替换元素**

    可替换元素:img,video,audio

    绝大部分可替换元素均为行盒

    特殊情况，可替换元素类似于行块盒，盒模型中所有尺寸都有效

    图片只设置宽度时，图片高会按比例增加
    object-fit:cover保证图片区域填充满不能有空隙，同时不能打破比例  content保证图片比例不变并且没有裁剪的去显示 fill保证图片填充满区域，不管比例