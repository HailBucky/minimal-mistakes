---

title:  "简单的svg动画"

---
 

## SVG动画的制作  

- 可以利用代码做出简单的动画效果

- 下面是沿着轨迹移动的动画

## 旋转着的爱心
- 以下是通过借鉴旋转效果做出来的简单SVG的代码

![heart.png](https://upload-images.jianshu.io/upload_images/9625930-dcbd97f3063f3ab9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 这个爱心不是svg的图片，而是通过文字功能中的特殊符号打出来的。虽然曾经想过是否要改变一下颜色，但是又觉得黑色蛮有特色的，也很可爱，就没有加入改变颜色的代码了。

<svg width="300" height="300" >
  <g> 
    <text font-family="microsoft yahei" font-size="120" y="120" x="100">❤</text>
    <animateTransform attributeName="transform" begin="0s" dur="10s" type="rotate" from="0 160 160" to="360 160 160" repeatCount="indefinite"/>
  </g>
</svg>


## 沿着一定轨道移动的音符
- 以下是代码的截图

![music.png](https://upload-images.jianshu.io/upload_images/9625930-5837954a7cb5c4ec.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

- 音乐音符和上面的爱心一样都是打出来的特殊符号
- 因为黑色有些单调，就更换成红色的了
- 一开始是有路径的痕迹的，但因为不美观所以删掉了

<svg width="360" height="200" >
  <text font-family="microsoft yahei" font-size="40" x="0" y="0" fill="#cd0000">♫
    <animateMotion path="M100,60 q100,120 120,20 q140,-50 160,0" begin="0s" dur="3s" rotate="auto" repeatCount="indefinite"/>
  </text>
  
</svg>
- 这个路径还是有点僵硬，一开始是想做成会旋转一圈的效果的，但调整了很久都还是失败了，所以最后只是做成了一个摇摆前进的小音符。