---
layout: post
title: CSSweb字体和图标
date: 2019-09-07 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
# web字体和图标

## web字体

用户电脑上没有安装相应字体，强制让用户下载改字体
使用@font-face制作新字体

```html
    <style>
        /* 制作一个新的web字体 */
        @font-face{
            font-family: "ppt";
            src:url("./font/一纸情书.TTF");
        }
        p{
            font-family: 'ppt';
        }
    </style>
```

## 字体图标

    https://iconfont.cn


## 在线字体图标

```html
<!DOCTYPE html>
<html lang="cmn-hans">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="//at.alicdn.com/t/font_1401358_jlr6jmtcc1.css">
    <style>
        /* 制作一个新的web字体 */
        @font-face{
            font-family: "ppt";
            src:url("./font/一纸情书.TTF");
        }
        p{
            font-family: 'ppt';
        }
    </style>
</head>
<body>
    <p>
        长夜将至，路漫漫其修远兮
        <i class="iconfont icon-yonghu1"></i>
    </p>
</body>
</html>
```

## 离线字体图标

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="./CSS/iconfont.css">
</head>
<body>
    <p>
        <i class="iconfont icon-yonghu2"></i>
    </p>
</body>
</html>
```

## Unicode方式引用字体图标

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style>
        @font-face {
            font-family: 'iconfont';
            src: url('./CSS/iconfont.eot');
            src: url('./CSS/iconfont.eot?#iefix') format('embedded-opentype'),
                url('./CSS/iconfont.woff2') format('woff2'),
                url('./CSS/iconfont.woff') format('woff'),
                url('./CSS/iconfont.ttf') format('truetype'),
                url('./CSS/iconfont.svg#iconfont') format('svg');
        }

        .iconfont {
            font-family: "iconfont" !important;
            font-size: 16px;
            font-style: normal;
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
        }
    </style>
</head>

<body>
    <i class="iconfont">&#xe602;</i>
</body>

</html>
```