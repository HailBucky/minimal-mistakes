---

title:  "较复杂的svg动画"

---



## SVG的制作
- 通过代码来制作一些图形（例如圆圈、矩形等）还算是相对容易的操作，但是不知道如何进一步的进行更加复杂的SVG动画的制作。

- 在网上找到了相关教程，自己试着进行重现。


## 跳动着的心
- 以下是代码截图。
![jumpingheart.png](https://upload-images.jianshu.io/upload_images/9625930-20187fdf482477de.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


- 通过增加style等来做出动画效果。
- 以下是动画呈现出的效果
<svg width="580" height="400" id="Capa_1" x="0px" y="0px" width="300px" height="300px" viewBox="0 0 60 60" style="enable-background:new 0 0 50 50;" xml:space="preserve" width="512px" height="512px">
  <g id="heart">
    <path style="fill:#C03A2B;" d="M24.85,10.126c2.018-4.783,6.628-8.125,11.99-8.125c7.223,0,12.425,6.179,13.079,13.543  c0,0,0.353,1.828-0.424,5.119c-1.058,4.482-3.545,8.464-6.898,11.503L24.85,48L7.402,32.165c-3.353-3.038-5.84-7.021-6.898-11.503  c-0.777-3.291-0.424-5.119-0.424-5.119C0.734,8.179,5.936,2,13.159,2C18.522,2,22.832,5.343,24.85,10.126z"/>
    <path style="fill:#ED7161;" d="M6,18.078c-0.553,0-1-0.447-1-1c0-5.514,4.486-10,10-10c0.553,0,1,0.447,1,1s-0.447,1-1,1  c-4.411,0-8,3.589-8,8C7,17.631,6.553,18.078,6,18.078z"/>
  </g>
</svg>
<style id="jsbin-css">
svg {

  width: 100%;
  margin: 0 auto;
  text-align: center;
}
#heart {
  animation-name: beat;
  animation-duration: 1s;
  animation-timing-function: ease;
  animation-iteration-count: infinite;
}
@keyframes beat {
  0% { 
    transform: scale(1);
  }
  50% {
    transform: scale(1.2);
  }
  100% {
    transform: scale(1);
  }
}
</style>
