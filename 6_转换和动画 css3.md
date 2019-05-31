**转换和动画 （css3）**



CSS3 转换，可以对元素进行移动、缩放、转动、拉长或拉伸。

 

**一、转换（2D）**

​      基于transform属性

​      取值：none  元素不进行转换

​               transform-function



​      transform-function:

​       1) rotate: 旋转

​           rotate（角度值）—deg

​           deg:正值  顺时针方向

​                  负值  逆时针方向

​           origin：数值、百分比、方向的关键字。

​                一个值：所有轴

​                二个值：x 、y

​                三个值：x、y、z

​               默认沿着元素中心

transform: rotate(30deg);//值 rotate(30deg) 把元素顺时针旋转 30 度。



​       2) translate: 移动

​           x y 轴移动的坐标位置

​           取值：a  数值、百分比。

​                    b  一个值：x

​                        两个值：x 、y

​                    c  正值：方向

translate(50px,100px);//值 translate(50px,100px) 把元素从左侧移动 50 像素，从顶端移动 100 像素。



​        3）scale: 改变元素尺寸、缩放

​             取值： a  数值

​                       b  放大>1

​                           缩小  0<1

​                       c  一个值：x与y轴都按这个值缩放

​                           两个值：x y的分别按各自的值缩放

transform: scale(2,4); //值 scale(2,4) 把宽度转换为原始尺寸的 2 倍，把高度转换为原始高度的 4 倍。



​       4) skew: 倾斜

​                skewX

​                skewY

​                skew(x,y)

transform: skew(30deg,20deg);//值 skew(30deg,20deg) 围绕 X 轴把元素翻转 30 度，围绕 Y 轴翻转 20 度。



5）matrix: 方法把所有 2D 转换方法组合在一起

matrix() 方法需要六个参数，包含数学函数，允许您：旋转、缩放、移动以及倾斜元素。		



![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/848d16092c3a4c4a8e7c8ae597a26549/clipboard.png)

通过网站演示：

**2d:**  

matrix(n,n,n,n,n,n)  <http://www.w3school.com.cn/tiy/c.asp?f=css_transform_matrix>

translate(x,y)  <http://www.w3school.com.cn/tiy/c.asp?f=css_transform_translate>

scale(x,y)   <http://www.w3school.com.cn/tiy/c.asp?f=css_transform_scale>

rotate(deg)  <http://www.w3school.com.cn/tiy/c.asp?f=css_transform_rotate>

skew(x-deg,y-deg)  <http://www.w3school.com.cn/tiy/c.asp?f=css_transform_skew>



**二、3D转换**

允许您使用 3D 转换来对元素进行格式化;

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/3eff3dbdf0a2474687f58ba5435cb09c/clipboard.png)







**三，过渡**

​      使得css 属性在一段时间内平滑的变化

​      transition：

​      参数: 1）过渡属性 

​                   all

​                   background

​                   color

​              2）过渡的时间

​                    以秒为单位，毫秒

​              3）过渡函数，过渡的速度

​                方式 

   linear：匀速

​                     ease：慢-快-慢

​                     ease-in：慢-快

​                     ease-out：快-慢

​                     ease-in-out：慢-快-慢

​     触发：hover、active、focus

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/3c5da8cb1dc24a0a939eb52a6e375691/clipboard.png)

例子：

```
div{

​	width:100px;

​	height:100px;

​	background:yellow;

​	transition-property:width 1s linear 2s;

}

div:hover{

​	width:200px;

}


```

**四，动画**

​      自动执行的过渡

​      animation：

​       1）-name:动画名称

​       2）-duration：动画持续的时间

​       3）-timing-function:动画函数

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/27bfae6ec442467fa36f05b94248a0d7/clipboard.png)

例子：

```
{

    width:100px;

    height:100px;

    background:red;

    position:relative;

    animation:myfirst 5s linear 2s infinite alternate;

}

@keyframes myfirst

{

    0%   {background:red; left:0px; top:0px;}

    25%  {background:yellow; left:200px; top:0px;}

    50%  {background:blue; left:200px; top:200px;}

    75%  {background:green; left:0px; top:200px;}

    100% {background:red; left:0px; top:0px;}

}



    animation-name: myfirst;

    animation-duration: 5s;

    animation-timing-function: linear;

    animation-delay: 2s;

    animation-iteration-count: infinite;

    animation-direction: alternate;

    animation-play-state: running;

等于

    animation:myfirst 5s linear 2s infinite alternate;
```

