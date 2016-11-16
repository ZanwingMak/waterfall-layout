# 瀑布流布局

**遇到了的问题和解决办法：**

1.如果图片未加载完，DIV高度不够导致图片重叠。（获取所有图片对象，轮询图片，加载完图片再执行回调函数来渲染瀑布流布局）

2.当高度不够时，没有滚动条。（第一次渲染完图片后，判断最短列的高度是否符合条件继续添加数据）

3.拖动滚动条时，执行了多次方法。（我是定义了个变量来判断是否允许再次执行加载数据的方法,但貌似没彻底解决?!）

Demo：http://demo.gfwboom.com/jquery/瀑布流布局/jquery.html

Github：https://github.com/maizhenying09/waterfall-layout

Blog：https://gfwboom.com/archives/code/jQuery/2016/11/16/jquery-waterfall-flow-layout.html

![image](https://gfwboom.b0.upaiyun.com/usr/uploads/2016/11/1939721335.jpg)
