### HTML5新特性
* 用于绘画的canvas元素
  SVG指可伸缩矢量图形 在任意分辨率下被高质量的打印
* 用于媒介回放的video和audio元素
  video和audio属性为视频和音频属性 ，通过设置source src为指定播放源 type为格式
* localStorage 用于长久保存整个网站的数据，没有时间限制，可手动删除
  sessionStorage 临时保存，关闭窗口或标签页删除这些数据
  保存localStorage.setItem(key,value)
  读取localStorage.getItem(key)
  单个删除localstorage.removeItem(key)
  全部删除localStorage.clear()
  获取key localStorage.key(index)
  同map
* 新的特殊内容元素
如：article、footer、header、nav、section
* 新的表单控件
如：calendar、data、time、Email、url、search

* 应用缓存 Application Cache
离线浏览 加载资源更快 减少服务器负载
* 启用应用程序缓存
```html
<html manifest="demo.appcache">
...
</html>
```
*
  manifest文件扩展名为'.appcache' 
  CACHE MANIFEST 首次下载时缓存文件 NETWORK 不会缓存 FALLBACK 页面无法访问是的回退界面
  第一行CACHE MANIFEST
  login.php 表示缓存login.php文件

### html元素
* html块元素
  块元素显示时，通常以新行开始
  如：`<h1>,<p>,<ul>`
* 内联元素
  不会以新行开始
  如: `<b>,<a>,<img>`
* Html`<div>`元素
  被看作快元素，只要是组合html元素的容器
* Html`<span> 元素元素，文本容器
* 单选框
  `<input type="radio" name="sex"/>` 需要加name
### html框架
* 框架标签（frame）
  框架对于页面的设计有着很大的作用
* 框架集标签（frameset）
  框架集标签定义如何将窗口分割为框架
  每一个frameset定义一些列行或列
  rows/cols的值规定每行或 每列占据屏幕的面积
* 常用标签
  noresize: 固定框架大小
  cols： 列
  rows： 行
* 内联框架iframe

* html target属性
<a href="http://www.baidu.com/"" target="_blank"></a>新窗口打开百度
_self 自身窗口 _parent 上层窗口 _top 顶层窗口 




























































































