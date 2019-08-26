---
layout: post
title: CSS常规流
date: 2019-09-01 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 常规流

    盒模型:规定单个盒子的规则

    视觉格式化模型(布局规则):页面中的多个盒子的排列规则

    视觉格式化模型，大体上将页面中盒子的排列分为三种方式

    1、常规流

    2、浮动

    3、定位

## 常规流布局
    常规流、文档流、普通文档流，常规流文档

    所有元素默认情况下都属于常规流

    总体规则:块盒独占一行，行盒水平依次排列

    包含块(containing block):每个盒子都有它的包含块，包含块决定了盒子的排列区域

    绝大部分情况下，盒子的包含块，为其父元素的内容盒

## 块盒

**1、每个块盒的总宽度，必须等于包含块的宽度**

    宽度的默认值是auto

    margin的取值也可以是auto，默认值为0

    auto:将剩余空间吸收掉

    width吸收能力强于margin

    若宽度、边框、内边距，外边距计算后，仍有剩余空间，该剩余空间被margin-right吸收

    在常规流中，块盒在包含块中居中方法，先定宽，然后margin左右为auto，

**2、每个块盒垂直方向上的auto值**

    heigh：auto，适应内容的高度

    margin: auto 表示0

**3、百分比取值**

    padding宽高 margin可以取值为百分比

    以上所有的百分比相对于包含块的宽度

    高度百分比:
        1、包含块的高度是否取决于子元素的高度，这种情况设置百分比无效

        2、包含块的高度不取决于子元素的高度，百分比相对于父元素高度

**4、上下外边距的合并**
    相邻兄弟元素或父子元素的上下margin会合并，
    兄弟元素 margin值为双倍，
    父子元素
    解决：1、只要隔开就好，如给父或子元素加border，
          2、父元素padding代替margin
