---

 
title:  "svg图片"

 
modified: 2018-07-07T16:03:49-04:00

 
categories: 

 
  - 网页设计

 
tags:

 
  - svg

 
---

 


 
{% include base_path %}

 


 
{% include toc title="Getting Started" %}

 
## SVG的定义  

- SVG意为**可缩放矢量图形**（Scalable Vector Graphics）

## 简单的svg动画


<svg width="500" height="500" xmlns="http://www.w3.org/2000/svg">
  <g> 
    <text font-family="microsoft yahei" font-size="120" y="120" x="100">svg</text>
    <animateTransform attributeName="transform" begin="0s" dur="10s" type="rotate" from="0 160 160" to="360 160 160" repeatCount="indefinite"/>
  </g>
</svg>