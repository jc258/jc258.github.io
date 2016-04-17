---
layout: post
title: "图片格式选择"
date: 2016-04-13 20:00:41
tags: [jpg, gif, png]
---

## 哪三种格式？

分别为：gif、jpg、png。

## 优化图像文件为何重要？

对于访问量不高的网站而言，图像的优化也许并不会引起我们太大的关注，但是如果日访问量都在数以万计的网站，简单举例是100000，那么某张图片的大小减小3k，一个月下来就节省了9G的带宽，这不管对于同时访问该网站的用户，还是网站运营本身来说，都将减少更少的开销。

## 不得不提及的几个概念。

1. 有损压缩与无损压缩
关于这两个概念，我在淘宝UED的blog上看到相关的文章《图片格式与设计那点事儿》，觉得很不错。

2. 色深
指某种图像格式包含的颜色的多少。用位表示，如8位色深表示256种颜色。

## 三种格式的简介

1. gif
- 只支持8位色深模式，即在同一张图像上只能存在256种颜色，如果超出，则某些颜色信息将丢失。
- 支持1位透明度，即要么全透明，要么不透明。
- 支持基于桢的简单动画（这是其他两种格式所不具备的）
- 何时可用？颜色值较少，有大块相同颜色区域的图像适合保存为此格式。

2. jpg
- 支持24位色深
- 不支持透明度
- 可对该格式的图像进行压缩，压缩的时候可设置等级。等级越高，图像越清晰，但是文件也就越大；反之亦然。所以在压缩的时候必须在图像质量和文件大小之间权衡利弊。
- 何时可用？颜色值较多，色彩和细节丰富的图像适合保存为此格式。

3. png
- 提供两种色深模式：8位和24位。
- 24位色深的png文件能做到无损压缩，但是文件也相应的会很大，并且在ie6下不被支持。
- 8位色深的png文件使用了类似gif的颜色索引，且在多数情况下，同等设置下用的png压缩的图像要比gif小。
- 何时可用？推荐使用8位色深的png文件。

## 结语

选择图像文件格式应该在透明度、色深、压缩率三者之间权衡一番，如果颜色色彩丰富，并且无需透明度支持，那么jgp无疑是最合适的选择；如果需要透明度支持，那么jpg无疑又是第一个得排除的选项。通过以上三种格式的简介，相信大家对怎么选择图像文件格式会有一定的了解的。