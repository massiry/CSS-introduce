**一、多列**

创建多个列来对文本进行布局类似报纸文本排版



![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/fafb3a8fc8084b539b3fcd5168b0bda5/clipboard.png)



例子：

```
.newspaper{

	width:300px;

	column-count:3;

}

<div>

    这个是测试内容 

    这个是测试内容 

    这个是测试内容

    这个是测试内容 

    这个是测试内容 

    这个是测试内容

    这个是测试内容 

    这个是测试内容 

</div>
```

效果：

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/482b22ab355b485eb35933c36990669e/clipboard.png)

**用户界面**

新的用户界面特性包括重设元素尺寸、盒尺寸以及轮廓等



**1.box-sizing**

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/f3e57680cedc4ce48c2950d0d4fe5400/clipboard.png)



**2.outline-offset**

outline-offset 属性对轮廓进行偏移，并在边框边缘进行绘制。



例子：div{

​	margin:20px;

​	width:150px; 

​	padding:10px;

​	height:70px;

​	border:2px solid black;

​	outline:2px solid red;

​	outline-offset:15px;

   } 

效果：

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/fbcd07bdaaa04801a7590c098c196741/clipboard.png)