---
title: 清风徐来
date: 2018-03-13 10:29:46
tags:
---
一，css 4种引用方式：
1，内联：<style></style> 标签
< style="” >  属性
2，外联   css  <link rel="stylesheet" href="./style.css”>
@import 在css文件中嵌套引用其他css文件

二，选择器:
1,类名选择器：
.className
2,标签选择器:
div
3,子类选择器
div>.className
4,子代选择器（.className是div的任意层级子类都可以找到，并不仅限为子类）
div .className

三，标签高度：高度由其内部文档流元素的高度的总和来决定。
文档流解释：文档内元素的流动方向，1，内联元素：从左往右如果遇到阻碍自动换行(允许单词可以换行word-break:break-all)。2，块级元素：从上往下。

四，脱离文档流(在计算高度时不纳入父标签高度计算，起始位置在父标签（0，0）开始)
方式：
1,{style：position: fixed;}
2，当前元素{style:position: absolute;}  ,  父类元素（参照元素）{style：position: relative;}

五，背景图片自适应
{style: background-position: center center;   （图片位置居中）
background-size: cover;    }            （图片大小适应当前控件）
六，内联元素不接受宽高，如：span。若想设置宽高则需要设置display：block

七，绝对位置（当脱离文档流设置绝对位置时）
top:100%  表示： 当前元素距离父元素的头部距离为父元素高度*100% ，也就是说在父元素的底部。
bottom：100%  表示：当前元素距离父元素的底部距离为父元素高度*100% ，也就是说在父元素的头部。

