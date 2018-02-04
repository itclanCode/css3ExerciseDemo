### 小鸟炫转

### 实现效果图如下所示
![小鸟炫转](img/小鸟炫转.gif)

### 实现代码
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>小鸟炫转</title>
    <style>
        *{
            margin:0;
            padding:0;
         }
         body{
            background:#27283b;
         }
         .bird{
            width:200px;
            height:200px;
            margin:100px auto;
            position:relative;
         }
         .bird .big{
            /* width: 10px;
            height: 10px; */
            /*border:100px solid transparent;*/
            position:absolute;
            /* border-top-color:blue;
            border-bottom-color:#f00cc;
            border-left-color:#66cc66;*/
            border-width:100px;
            border-style:solid;
            border-color:transparent transparent #d72928 #db3e3d;
            left:0;
            top:0;
            border-radius:50%;
            transform:rotate(45deg);
            transition:all 0.2s ease;
         }
         .middle{
            border-width:80px;
            border-style:solid;
            border-color:#f8d245 transparent #f2f2f2 #fff;
            position:absolute;
            left:10%;
            top:10%;
            border-radius:50%;
            transform:rotate(45deg);
         }
         .small{
            border-width:40px;
            border-style:solid;
            border-color:transparent #f7a703 transparent transparent;
            border-radius:50%;
            transform:rotate(45deg);
            position:absolute;
            left:30%;
            top:30%;
         }
         .small:before{  /* 小黑原点 */
            content:"";
            width:20px;
            height:20px;
            background:#000;
            border-radius:50%;
            position:absolute;
            top:-10px;
            right:20px;
         }
         .bird:hover .big{
            transform:rotate(225deg);
            border-color:transparent transparent #1fe8b6 #16d7a7;
            transition:all 0.2s ease;
            cursor:pointer;
         }
         .bird:hover .middle{
            transform:rotate(-135deg);/* 逆时针炫转135度 */
            border-color:transparent #f8d245 #fff #f2f2f2;
            transition:all 0.2s ease;
            cursor:pointer;
         }
         .bird:hover .small{ /* 小眼睛 */
            transform:rotate(135deg);
            transition:all 0.2s ease;
            cursor:pointer;
         }
    </style>
</head>
<body>
       <div class="bird">
             <div class="big"></div><!-- 最外面的红色的圆圈 -->
             <div class="middle"></div><!--中间白色的圈,黄色的圈,灰色的圈-->
             <div class="small"></div><!--小嘴巴-->
       </div>
</body>
</html>
<!--
    伪类:相当于是在盒子里面添加行内元素

-->

```

### 实现原理
* 若干个圆来实现的
* 三角形的制作,透明背景transparent
* 左边一个红色半圆,右边右边一个圆(三角),绝对定位盖在红色的圆上面,中间的眼睛是巧妙的用伪类来做的
* 通过鼠标移入移出,移到哪个元素上面,就会发生炫转和变化


