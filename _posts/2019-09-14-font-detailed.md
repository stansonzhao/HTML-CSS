---
layout: post
title: CSS深入理解字体
date: 2019-09-14 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 参考线-深入理解字体

    font-size line-height vertical-align font-family

## 文字

    文字时通过一些文字制作软件制作的，比如fontforge

    制作文字时，会有几根参考线，不同的文字类型，参考线不一样。同一种文字参考线一致

    字体制作参考线有text top/ascent,顶线。 super,上基线。 baseline，基线。 sub,下基线。 textbottom,descent 底线。

![基线]({{site.baseurl}}/assets/img/ppt-image.png)

## font-size

    字体大小，设置的是文字的相对大小

    文字相对大小:1000、2048、1024

    文字的顶线到底线距离是文字的实际大小，叫做(content area 内容区)

    行盒背景覆盖内容区

## 行高 

    顶线向上延申的空间和底线向下延申的空间，两个空间相等，该空间叫做空隙(gap)

    gap默认情况下是字体设计者决定的

    top到bottom(看PTT图片)区域距离叫做virtual-area(虚拟区)，往往会高于内容区

    行高就是virtual-area

    line-height:normal,默认值，使用文字默认的gap

## vertical-align

    决定参考线的:font-size font-family line-height

    一个元素的子元素出现行盒，该元素的内部也会产生参考线

    baseline:该元素的基线与父元素的基线对齐

    super:表示该元素的基线与父元素的上基线对齐

    sub:表示该元素的基线与父元素的下基线对齐

    top:该元素的virtual-area顶边，对齐line-box的顶边

    bottom:该元素的virtual-area底边，对齐line-box的底边

    middle:该元素的中线（content-area的一半），与父元素的X字母高度一半的位置对齐

    行盒组合起来，可以形成多行，每一行的区域叫做line-box,line-box的顶边是该行内所有行盒最高顶边，底边该行行盒的最低底边

    实际，一个元素的实际占用高度(高度自动)，高度的计算通过line-box计算

    行盒:inline-box
    行框:line-box

    数值：相对于基线的偏移量，向上为正数，向下为负数

    百分比：相对于基线的偏移量，百分比是相对于自身virtual-area的高度

    line-box是承载文字内容的必要条件，以下情况不生成行框：
        1、某元素内部没有任何行盒
        2、某元素字体大小为0

## 可替换元素和行块盒的基线

    图片:基线位置位于图片的下外边距

    表单元素:基线位置在内容底边

    行块盒：
        1、行块盒最后一行有line-box，用最后一行的基线作为整个行块盒的基线
        2、如果行块盒内部最后一行没有行盒，则使用底下外边距作为基线