---
layout: post
title: CSS常见样式属性
date: 2019-08-24 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# 常见样式属性
    1、color
        元素内部文字颜色
        可填值
            预设值：定义好的单词
            三原色(色值)：red，green，blue。每个颜色可通过0~255数值来表示，数值越大改颜色越浓

```
RGB表示法：
rgb(0，0，0);表示黑色rgb(255,255,255);表示白色
hex16进制表示法:
每一种颜色用两位数来表示，诺同一色中两位数相同可简写为一位，如#ff4400;可缩写为#f40
#红绿蓝 马尔斯绿：#008c8c,
淘宝红：#f40
白色：#fff
黑色：#000
红：#f00
绿：#0f0
蓝：#00f
紫：#f0f
青:#0ff
黄色：#ff0
灰色：#ccc
```

    2、background-color
        元素背景颜色
    3、font-size
        元素内部文字尺寸大小
            单位：
                1、px(像素)
                2、em(相对字体大小，相对父元素字体大小)
                每个元素必须要有字体大小，如果没有声明字体大小，则直接使用父元素字体大小，如果没有父元素(html)则使用基准字号，基准字号由浏览器设置。uesr agent 用户代理(浏览器)
    4、font-weight
        文字粗细程度
            可取值为数字或预设值
                预设值有：normal,bold,bolder
        strong默认样式是加粗字体，通常开发中strong用来表示重要的不能忽略的内容。
    5、font-family
        文字字体，必须是用户计算机中存在的字体才有效
        使用多种字体以匹配不同环境，每种字体之间用逗号隔开
            sans-serif，非衬线字体
            衬线字体是对字体笔画边缘有修饰的字体，如宋体
            打印纸张用衬线字体。网页显示用非衬线字体。
        字体中加入sans-serif做兼容显示
    6、font-style
        字体样式，通常用它设置斜体(italic)
        i元素默认样式是倾斜字体，实际使用通常用它表示一个图标
        em元素默认是斜体，开发中用来表示强调内容

    7、text-decoration
        文本修饰(给文本加线)
            值有:none(没有线)
                line-through(穿过文字中间加条线，中划线)
                over-line(上边加线，上划线，用的少)
                underline(文字下方加条线，下划线，用的多)
        del元素(表达错误的内容)
        s元素(过期的元素)
    8、line-height
        行高,值越大，每行文本的距离越大
        设置行高为容器的高度，可以让单行文本垂直居中
        行高可以设置为纯数字，表示相对于当前元素的字体大小
            单位：像素

    9、width
        容器宽度
    10、height
        容器高度
            单位：px或百分比
    11、letter-space
        文字间隙
            单位：像素或em
    12、text-indent
        text-indent(首行缩进)单位为em，相对单位，表示缩进多少个文字，px为单位表示缩进多少像素
    13、text-align
        元素内部，让文字水平排列
    14、font
        设置简写属性
        后可以跟font-size,font-variant,font-weigth,font-size,line-heigth,font-family
    15、font-variant:small-caps(小型大写字母)
        将小写字母改为大写