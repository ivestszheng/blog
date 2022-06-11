# 长列表无限下拉的实现（下）

## 前言

还没看过的小伙伴，先看下上篇[《长列表无限下拉的实现（上）》](https://juejin.cn/post/7106145431893065736)。

## 不定高元素虚拟列表的实现

### 整体思路

我的方案是自定义一个 `estimatedHeight` 属性对行高进行估计并渲染，渲染完成后获得真实行高并进行更新和缓存。

此外，我看到手淘的一个方案是通过`intersectionObserver`获取进入到视口的元素，具体可以看这篇文章[《无限滚动加载解决方案之虚拟滚动（下）》](https://blog.csdn.net/Taobaojishu/article/details/121173387)。

## 存在的问题

## 总结

## Demo地址

[ivestszheng/virtual-scroll-demo](https://github.com/ivestszheng/virtual-scroll-demo)。

## 参考资料

1. [云+社区 -「前端进阶」高性能渲染十万条数据(虚拟列表)](https://cloud.tencent.com/developer/article/1533206)
3. [csdn - 无限滚动加载解决方案之虚拟滚动（下）](https://blog.csdn.net/Taobaojishu/article/details/121173387)