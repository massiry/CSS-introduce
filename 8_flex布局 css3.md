**一、Flex布局**

flex Flex是Flexible Box的缩写，意为”弹性布局”，用来为盒状模型提供最大的灵活性。任何一个容器都可以指定为Flex布局。

 

**二、基本概念**

采用Flex布局的元素，称为Flex容器（flex container），简称”容器”。它的所有子元素自动成为容器成员，称为Flex项目（flex item），简称”项目”。



**三、容器的属性**

**1****.****flex-direction**   决定主轴的方向（即项目的排列方向）

属性值:

row（默认值）：主轴为水平方向，起点在左端。

row-reverse：主轴为水平方向，起点在右端。

column：主轴为垂直方向，起点在上沿。

column-reverse：主轴为垂直方向，起点在下沿。



**2.****flex-wrap**  决定项目是否换行

属性值:

nowrap（默认）：不换行。

wrap：换行，第一行在上方。

wrap-reverse：换行，第一行在下方。



**3.flex-flow**  flex-direction属性和flex-wrap属性的简写形式，默认值为row nowrap。



**4.****justify-content**   定义了项目在主轴上的对齐方式。

属性值:

flex-start（默认值）：左对齐

flex-end：右对齐

center： 居中

space-between：两端对齐，项目之间的间隔都相等。

space-around：每个项目两侧的间隔相等。所以，项目之间的间隔比项目与边框的间隔大一倍。



**5.align-items**  定义项目在交叉轴上如何对齐

属性值：

flex-start：交叉轴的起点对齐。

flex-end：交叉轴的终点对齐。

center：交叉轴的中点对齐。

baseline: 项目的第一行文字的基线对齐。

stretch（默认值）：如果项目未设置高度或设为auto，将占满整个容器的高度。



**6.****align-content**  定义了多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用。

属性值：

flex-start：与交叉轴的起点对齐。

flex-end：与交叉轴的终点对齐。

center：与交叉轴的中点对齐。

space-between：与交叉轴两端对齐，轴线之间的间隔平均分布。

space-around：每根轴线两侧的间隔都相等。所以，轴线之间的间隔比轴线与边框的间隔大一倍。

stretch（默认值）：轴线占满整个交叉轴。



**四、项目的属性**

**1.order**  定义项目的排列顺序。数值越小，排列越靠前，默认为0。



**2.flex-grow** 定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。

如果所有项目的flex-grow属性都为1，则它们将等分剩余空间（如果有的话）。如果一个项目的flex-grow属性为2，其他项目都为1，则前者占据的剩余空间将比其他项多一倍。



**3.flex-shrink** 定义了项目的缩小比例，默认为1，即如果空间不足，该项目将缩小。

如果所有项目的flex-shrink属性都为1，当空间不足时，都将等比例缩小。如果一个项目的flex-shrink属性为0，其他项目都为1，则空间不足时，前者不缩小。

负值对该属性无效。



**4.flex-basis** 定义了在分配多余空间之前，项目占据的主轴空间（main size）。浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。

它可以设为跟width或height属性一样的值（比如350px），则项目将占据固定空间。



**5.flex**  是flex-grow, flex-shrink 和 flex-basis的简写，默认值为0 1 auto。后两个属性可选。

该属性有两个快捷值：auto (1 1 auto) 和 none (0 0 auto)。建议优先使用这个属性，而不是单独写三个分离的属性，因为浏览器会推算相关值



**6.align-self** 允许单个项目有与其他项目不一样的对齐方式，可覆盖align-items属性。默认值为auto，表示继承父元素的align-items属性，如果没有父元素，则等同于stretch。

属性值：

auto: 将占满整个容器的高度。

flex-start：交叉轴的起点对齐。

flex-end：交叉轴的终点对齐。

center：交叉轴的中点对齐。

baseline: 项目的第一行文字的基线对齐。

stretch：如果项目未设置高度或设为auto，将占满整个容器的高度。





参考文章：<https://www.runoob.com/w3cnote/flex-grammar.html>

   <http://www.ruanyifeng.com/blog/2015/07/flex-examples.html>

flex在线演示：<https://www.html.cn/demo/flexbox-playground/>

![img](C:/Users/yafei/AppData/Local/YNote/data/m15508511041_1@163.com/5a58ce3ee9b141ed99a4ed4caf65e1a3/image.jpg)