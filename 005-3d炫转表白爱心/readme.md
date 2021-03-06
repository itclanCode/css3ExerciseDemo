### 3d炫转表白爱心

### 实效果如下
![表白爱心](img/表白爱心.gif)


### 实例代码

```
<!doctype html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="Keywords" content="关键词">
        <meta name="Description" content="描述">
        <title>Document</title>
        <style>/*css样式表的衣柜*/
        *{margin:0px;padding:0px;}/*去除默认外边距、内边距*/
        body{background:#000;}
        .heart{
            width:100px;
            height:160px;
            position:absolute;
            left:0px;
            top:0px;
            right:0px;
            bottom:0px;
            margin:auto;
            transform-style:preserve-3d;
            animation:play 10s infinite linear;/*自定义动画：名称
        时间  无限重复 匀速运动*/
        }
        @keyframes play{
            to{transform:rotateX(360deg) rotateY(360deg);}
        }
        .heart [class^="heart"]{width:100px;height:160px;
        border:solid red;position:absolute;
        border-width:2px 2px 0 0;
        border-radius:50% 50% 0%/40% 50% 0%;/*前面四个值是水平方向/后面的四个值是垂直方向*/
        }
        .heart [class$="1"]{
            transform:rotateY(10deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="2"]{
            transform:rotateY(20deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="3"]{
            transform:rotateY(30deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="4"]{
            transform:rotateY(40deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="5"]{
            transform:rotateY(50deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="6"]{
            transform:rotateY(60deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="7"]{
            transform:rotateY(70deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="8"]{
            transform:rotateY(80deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="9"]{
            transform:rotateY(90deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="10"]{
            transform:rotateY(100deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="11"]{
            transform:rotateY(110deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="12"]{
            transform:rotateY(120deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="13"]{
            transform:rotateY(130deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="14"]{
            transform:rotateY(140deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="15"]{
            transform:rotateY(150deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="16"]{
            transform:rotateY(160deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="17"]{
            transform:rotateY(170deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="18"]{
            transform:rotateY(180deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="19"]{
            transform:rotateY(190deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="20"]{
            transform:rotateY(200deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="21"]{
            transform:rotateY(210deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="22"]{
            transform:rotateY(220deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="23"]{
            transform:rotateY(230deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="24"]{
            transform:rotateY(240deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="25"]{
            transform:rotateY(250deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="26"]{
            transform:rotateY(260deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="27"]{
            transform:rotateY(270deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="28"]{
            transform:rotateY(280deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="29"]{
            transform:rotateY(290deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="30"]{
            transform:rotateY(300deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="31"]{
            transform:rotateY(310deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="32"]{
            transform:rotateY(320deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="33"]{
            transform:rotateY(330deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="34"]{
            transform:rotateY(340deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="35"]{
            transform:rotateY(350deg) rotateZ(45deg) translateX(30px);
        }
        .heart [class$="36"]{
            transform:rotateY(360deg) rotateZ(45deg) translateX(30px);
        }
        .img{
            width:50px;
            height:50px;
            transform-style:preserve-3d;  /*构建3d坏境*/
            position:absolute;
            left:0px;
            top:0px;
            right:0px;
            bottom:0px;
            margin:auto;
            transform:translateZ(22px);}
        .img div{
            width:50px;
            height:50px;
            position:absolute;
            background-size:100% 100% !important;
        }
        .img div:nth-child(1){
            left:0px;
            top:-50px;
            transform:rotateX(90deg);
            background:url(images/1.jpg);
            transform-origin:bottom;
        }
        .img div:nth-child(2){
            left:0px;
            top:50px;
            transform:rotateX(-90deg);
            background:url(images/2.jpg);
            transform-origin:top;
        }
        .img div:nth-child(3){
            left:-50px;
            top:0px;
            background:url(images/3.jpg);
            transform-origin:right;
            transform:rotateY(-90deg);}
        .img div:nth-child(4){
            left:50px;
            top:0px;
            background:url(images/4.jpg);
            transform-origin:left;
            transform:rotateY(90deg);
        }
        .img div:nth-child(6){
            left:0px;
            top:0px;
            background:url(images/5.jpg);
        }
        .img div:nth-child(5){
            left:0px;
            top:0px;
            background:url(images/6.jpg);
            transform:translateZ(-50px)
        }
        </style>
    </head>
    <body><!--身体-->
        <div class="heart">
            <div class="heart1"></div>
            <div class="heart2"></div>
            <div class="heart3"></div>
            <div class="heart4"></div>
            <div class="heart5"></div>
            <div class="heart6"></div>
            <div class="heart7"></div>
            <div class="heart8"></div>
            <div class="heart9"></div>
            <div class="heart10"></div>
            <div class="heart11"></div>
            <div class="heart12"></div>
            <div class="heart13"></div>
            <div class="heart14"></div><div class="heart15">
</div>
            <div class="heart16"></div>
            <div class="heart17"></div>
            <div class="heart18"></div>
            <div class="heart19"></div>
            <div class="heart20"></div>
            <div class="heart21"></div>
            <div class="heart22"></div>
            <div class="heart23"></div>
            <div class="heart24"></div>
            <div class="heart25"></div>
            <div class="heart26"></div>
            <div class="heart27"></div>
            <div class="heart28"></div>
            <div class="heart29"></div>
            <div class="heart30"></div>
            <div class="heart31"></div>
            <div class="heart32"></div>
            <div class="heart33"></div>
            <div class="heart34"></div>
            <div class="heart35"></div>
            <div class="heart36"></div>
            <div class="img">
                <div></div>
                <div></div>
                <div></div>
                <div></div>
                <div></div>
                <div></div>
            </div>
        </div>
</body>
```
### 实现原理
* 线条是用边框做的,有一个弯曲的线,border-radius,通过后面的8个值来得到的
* border-radius:4px 4px 4px 4px/5px 5px 5px 5px 前面四个是水平方向的,后面四个是垂直方向的
* 弯曲的线条是若干条线组合而成的,让它在一个y轴方向有一个炫转
