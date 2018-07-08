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

- 下面是沿着轨迹移动的动画

##旋转着的

<svg width="500" height="500" >
  <g> 
    <text font-family="microsoft yahei" font-size="120" y="120" x="100">❤</text>
    <animateTransform attributeName="transform" begin="0s" dur="10s" type="rotate" from="0 160 160" to="360 160 160" repeatCount="indefinite"/>
  </g>
</svg>


## 沿着一定轨道移动的音符

<svg width="360" height="200" >
  <text font-family="microsoft yahei" font-size="40" x="0" y="0" fill="#cd0000">♫
    <animateMotion path="M100,60 q100,120 120,20 q140,-50 160,0" begin="0s" dur="3s" rotate="auto" repeatCount="indefinite"/>
  </text>
  
</svg>
