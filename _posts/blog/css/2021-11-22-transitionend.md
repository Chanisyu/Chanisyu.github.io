---
layout: post
title: css 模拟长按事件
categories: [CSS]
description: css 模拟长按事件
keywords: css 模拟长按事件
---

# 背景
 在app端常有的操作就是长按，长按之后手机有一些操作。那么在移动端也想实现这种长按的操作，怎么做呢？

## js实现方式
因为原生的js是没有长按事件的，可能大多数人想的是用 `touchStart` , `touchMove` , `touchEnd` 进行模拟。手指按下开始计时，在判断在手指按下的过程中否有x或者y方向的移动（区分移动还是长按），如果有x或者y轴的移动距离很大就不是长按，没有的话就是长按。当满足条件的时候， 手指离开，就可以在 `touchEnd` 里面做一些操作了，从而实现了长按。

具体的代码不在细细诉说，可以自己实现一版。gan sho