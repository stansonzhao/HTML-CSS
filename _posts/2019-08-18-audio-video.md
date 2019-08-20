---
layout: post
title: HTML之多媒体元素
date: 2019-08-18 15:30:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
Hyper Text Markup Language, an application under the standard universal markup language. HTML is not a programming language, but a markup language that is essential for web page creation.

Cascading Style Sheets (English name: Cascading Style Sheets) is a computer language used to represent file styles such as HTML (an application of the standard universal markup language) or XML (a subset of the standard universal markup language).
# 多媒体元素
    video 视频
    audio 音频
## video
    controls:控制播放控件的显示，写值得话，值只能为controls
    某些属性只有两种状态，要么不写属性，要么写了值为属性名(缩写只写属性名，这种属性叫布尔属性。
    可缩写，只写属性名
    autoplay:布尔属性，自动播放
    muted:布尔属性，静音播放
    loop:布尔属性，循环播放
## audio
    属性和视屏一致
## 兼容性
    1、旧版本浏览器不支持这两个元素
    2、不通的浏览器支持的音视频格式可能不同

    MP4、webm

```html
<!--代码-->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>
    <video loop muted autoplay controls>
        <source src="233.mp4"> 浏览器兼容，浏览器识别到mp4就不会播放webm的视频，识别不到MP4则播放webm的视频
        <source src="233.webm">
    </video>
</body>
</html>
```