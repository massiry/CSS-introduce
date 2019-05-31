**CSS3 渐变（gradients）可以让你在两个或多个指定的颜色之间显示平稳的过渡。**



**CSS3 定义了两种类型的渐变（gradients）：**

线性渐变（Linear Gradients）- 向下/向上/向左/向右/对角方向

径向渐变（Radial Gradients）- 由它们的中心定义

 

渐变色存在着兼容性问题所有在使用的时候需要加上兼容前缀：



线性渐变效果：

<div id="grad"></div>

\#grad {

​    height: 200px;

​    background: -webkit-linear-gradient(red, blue); /* Safari 5.1 - 6.0 */

​    background: -o-linear-gradient(red, blue); /* Opera 11.1 - 12.0 */

​    background: -moz-linear-gradient(red, blue); /* Firefox 3.6 - 15 */

​    background: linear-gradient(red, blue); /* 标准的语法（必须放在最后） */

}

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/3b60c4cdee2d41598224441e675b76db/clipboard.png)



径向渐变效果：

<div id="grad1"></div>

\#grad1 {

​    height: 150px;

​    width: 200px;

​    background: -webkit-radial-gradient(red, green, blue); /* Safari 5.1 - 6.0 */

​    background: -o-radial-gradient(red, green, blue); /* Opera 11.6 - 12.0 */

​    background: -moz-radial-gradient(red, green, blue); /* Firefox 3.6 - 15 */

​    background: radial-gradient(red, green, blue); /* 标准的语法（必须放在最后） */

}

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/6dba5b304721497298a17f42e7a939c0/clipboard.png)



```
**1.线性渐变**

​     linear-gardient( to bottom,color,color )

​     linear-gardient(angle,color-point1,color-point2......)

​     angle:角度，指定渐变的方向，可以是角度值，也可以是关键字

​     0deg to  top

​     90deg to right

​     180deg to b         ottom

​     270deg to left

​     color-point:颜色，颜色的范围

**2.颈向渐变**

​     radial-gradient([size at position],color-point )

[size at position]: 第一参数指定渐变的圆心位置，还有size，默认为center

​     color-point

**3.重复线性渐变**

​     repeating-linear-gradient;

​     里面的参数值和线性渐变一样

**4.重复颈向渐变**

​     里面的参数值和颈向渐变一样

​     repeating-radial-gradient;
```

