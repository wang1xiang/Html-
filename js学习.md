#### 函数属性和方法
* 函数有length属性 表示函数接收的参数个数
* 函数有prototype属性，每个函数都有两个非继承而来的方法：apply()和call()
1、设置函数体this对象值
apply() 接收两个参数，第一个this对象，第二个arguments或数组 sum.apply(this,arguments)
call() 第二个参数直接传递 sum.call(this,num1,num2)
2、扩充函数的运行的作用域
  ```javascript
  window.color="red"
  var o={color:"blue"}
  function sayColor(){
    console.log(this.color)
  }
  sayColor()  red
  sayColor.call(this) red
  sayColor.call(o) blue
```
* es5新增bind()方法，创建一个函数的实例，this值绑定到传给bind()函数的值
  ```javascript
  var objectsay = sayColor.bind(o)
  objectsay() blue:
  ```
#### 基本封装类型
#### string类型
* slice() substr() substring() 第一个参数指定字符串开始位置
区别
  slice()和substring() 第二个参数指定最后一个字符后的位置，而substr()指定返回的字符个数
* 字符串匹配
  match()接收正则表达式或字符串 匹配不到返回null
  ```javascript
  let a="cat,bat,sat,fat"
  let pattern = /.at/
  let matchs = a.match(pattern)
  matchs ["cat", index: 0, input: "cat,bat,sat,fat"]
  ```
  search() 返回匹配到的索引，匹配不到返回-1
  ```javascript
  search = b.search(/at/)
  1
  search = b.search('g')
  -1
  ```
* 字符串替换
  replace()第一个参数为字符串，只能匹配第一个结果，匹配全局使用正则表达式，指定全局(g)
  ```javscript
  search = b.replace(/at/g,'ond')
  "cond,bond,sond,fond"
  ```