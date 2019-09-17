---
layout: post
title: CSS行高取值
date: 2019-09-11 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 行高的取值
    line-height

    1、px，像素值。
        仅适用于单行文本
        先计算像素值，再继承
        行高定死，当字体大小改变时，行高不会变

    2、无单位数值
        适用多行不同文本
        先继承再计算
    3、em单位
        先计算像素值，再继承
        行高为当前元素字体大小的两倍。先计算，再继承

    4、百分比
        先计算像素值，再继承
        与em意思一样，先计算，再继承