---

title:  "简单的svg动画"

 
modified: 2018-07-07T16:03:49-04:00

 
categories: 

 
  - 网页设计

 
tags:

 
  - svg
classes: wide
---

 
{% include base_path %}
 
{% include toc title="Getting Started" %}

{% include gallery caption="This is a sample gallery with **Markdown support**." %}

## SVG动画的制作  

- 可以利用代码做出简单的动画效果

## 沿着一定轨道移动的音符

<svg width="360" height="200" xmlns="http://www.w3.org/2000/svg">
  <text font-family="microsoft yahei" font-size="40" x="0" y="0" fill="#cd0000">♫
    <animateMotion path="M100,60 q100,120 120,20 q140,-50 160,0" begin="0s" dur="3s" rotate="auto" repeatCount="indefinite"/>
  </text>
  
</svg>
