#### js数据类型
1、字符串(String)
2、数字(Number)
3、布尔(Boolean)
4、数组(Array)
5、对象(Object)
6、空(null)
7、未定义(undefined)
* 可以通过赋值为null的方式清除变量
#### 比较运算符
* 双等号值相等就行 '10' == 10 true
* 三等号值和类型都相等 '10' === 10 false
#### Dom操作css
* document.getElementById(id).style.property = new style
#### Dom EventListener
* addEventListener(event, function,'布尔值') true事件捕获 false 事件冒泡 removeEventListener
 添加多个不会覆盖
* 事件流：描述页面中接受事件的顺序
* 事件冒泡：由子元素向父级传播
* 事件捕获：由父级向子元素传播
#### 事件对象
* 触发dom事件会产生一个对象event
1、type：获取事件类型
2、target：获取事件目标
3、stopPropagation()：阻止事件冒泡
4、preventDefault()：阻止事件默认行为
* let m = time.getMinutes().toString().padStart(2,'0') // 前面补0
#### window对象
* window对象是bom的核心，指当前的浏览器窗口
  全局对象是window对象属性、函数是window对象方法
  window.innerHeight 浏览器窗口的内部高度
  window.innerWidth 浏览器窗口的内部宽度
#### Screen对象
* window.screen 对象包含有关用户屏幕的信息
  screen.availWidth 可用宽度
  screen.availHeight 可用高度
  screen.Width 屏幕宽度
  screen.Height 屏幕高度

#### nodejs
* 应用领域
 RESTFul API
 实时通信: 如消息推送等
 高并发
 i/o阻塞
* nodejs特点
 部署简单方便  只需安装Node.js即可
 事件驱动 根据当前事件 进行资源调动
 异步编程 
 高效与性能
 单线程与多线程 
 V8是单线程，所以Node.js也是单线程的，为了更好利用CPU资源，可以利用子进程和多进程
 子进程：Node.js的child_process模块
 多进程：PM2等第三方工具
 nodejs的缺点
 大量使用匿名函数，抛出的异常不易阅读
 try/catch限于同步代码，是的异常捕获较为复杂
 单线程：可靠性
 不适合CPU密集型的场景