.container {
    display: flex | inline-flex;       //可以有两种取值
}
# 需要注意的是：当时设置 flex 布局之后，子元素的 float、clear、vertical-align 的属性将会失效。

# 有下面六种属性可以设置在容器上，它们分别是：

1. flex-direction: 决定主轴的方向(即项目的排列方向)
    flex-direction: row | row-reverse | column | column-reverse;
2. flex-wrap: 决定容器内项目是否可换行
    flex-wrap: nowrap | wrap | wrap-reverse;
3. flex-flow: flex-direction 和 flex-wrap 的简写形式   (排列方式)
    flex-flow: <flex-direction> || <flex-wrap>; 默认值为: row nowrap
4. justify-content：定义了项目在主轴的对齐方式。 (水平对齐)
    justify-content: flex-start | flex-end | center | space-between | space-around;
5. align-items: 定义了项目在交叉轴上的对齐方式   (垂直对齐)
    align-items: flex-start | flex-end | center | baseline | stretch;
6. align-content: 定义了多根轴线的对齐方式，如果项目只有一根轴线，那么该属性将不起作用  (多行对齐)
    align-content: flex-start | flex-end | center | space-between | space-around | stretch;
# 有六种属性可运用在 item 项目上：
1. order: 定义项目在容器中的排列顺序，数值越小，排列越靠前，默认值为 0
    order: <integer>;
2. flex-basis: 定义了在分配多余空间之前，项目占据的主轴空间，浏览器根据这个属性，计算主轴是否有多余空间
    flex-basis: <length> | auto;  0% or auto
3. flex-grow: 定义项目的放大比例
    flex-grow: <number>; 默认值为 0，即如果存在剩余空间，也不放大,flex-grow 属性为 2，其他项目都为 1，则前者占据的剩余空间将比其他项多一倍。
4. flex-shrink: 定义了项目的缩小比例
    flex-shrink: <number>;默认值: 1，即如果空间不足，该项目将缩小，负值对该属性无效。flex-shrink 属性为 0，其他项目都为 1，则空间不足时，前者不缩小
5. flex: flex-grow, flex-shrink 和 flex-basis的简写
    flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]默认值是 0 1 auto。
6. align-self: 允许单个项目有与其他项目不一样的对齐方式
    align-self: auto | flex-start | flex-end | center | baseline | stretch;

     https://zhuanlan.zhihu.com/p/25303493
