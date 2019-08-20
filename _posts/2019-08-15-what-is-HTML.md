---
layout: post
title: 基础HTML结构由哪些构成
date: 2019-08-15 16:32:20 +0000
description: 什么是HTML?什么是CSS？. # Add post description (optional)
img: html-1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [CSS, HTML]
---
Hyper Text Markup Language, an application under the standard universal markup language. HTML is not a programming language, but a markup language that is essential for web page creation.

Cascading Style Sheets (English name: Cascading Style Sheets) is a computer language used to represent file styles such as HTML (an application of the standard universal markup language) or XML (a subset of the standard universal markup language).

# 第一个网页
    Emmet自动生成HTML代码片段
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

## 注释
    注释是为代码的阅读者提供帮助
    HTML中的注释使用如下格式书写
```html
    <!--注释内容-->
 ```

## 元素
```html
<a href="http://www.syics.com">信息咨询服务</a>
```
    官方称element为元素
    元素 = 起始标记(begin tag) + 元素内容 + 元素属性 + 结束标记(end tag)
    属性 = 属性名 + 属性值
    属性的分类：
        局部属性：某些元素特有的属性
        全局属性：这些属性所有元素通用
    有些元素没有结束标记，这样的元素叫做：**空元素**
空元素的两种写法：
```html
        1、<mate charset = "utf-8">
        2、<mate charset = "utf-8"/>
```

## 元素嵌套
```html
元素不能相互嵌套如:
    <div>
        <p>
        </div>
    </p>
```

## 标准的文档结构
HTML：页面，HTML文档
```html
    这个叫做文档声明
    <!DOCTYPE html>
```

lang：语言，代表改HTML文档的语言类别
```html
    cmn:中国官方语言  han：汉语 s:简体
    <html lang="cmn-hans">
```