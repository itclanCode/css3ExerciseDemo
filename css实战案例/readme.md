### 表单美化

表单的用途

* 登录
* 注册
* 搜索

### 需要用到的控件
* text 
* password
* radio
* checkbox
* textarea 
* button

background-size:背景的大小
cover 覆盖
会铺满当前的屏幕
filter:blur();滤镜,针对的是它里面的所有元素.默认是0像素

background-clip背景裁切
-border-box: 默认 
-padding-box
-content-box 

盒模型
border  边框区域
padding 内填充
content 内容区域

线性渐变
background:linear-gradient({
    to top,
    red,
    green,
    blue
})
to top,从下而上
to bottom 从上而下
to left  从右到左
to right 从左到右
----------------
display:flex 弹性盒模型
flex: 宽度

根据当前宽度到富裕宽度(剩余可利用空间)/flex总和 = 1 取其中到一份

