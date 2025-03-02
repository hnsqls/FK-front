# JavaScript

## 入门

js就是脚本文件，可以动态的修改html的内容。

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>js入门</title>
</head>
<body>

    <p id="p1">11111</p>
    
</body>
</html>
```

修改  1111 --> 2222

![image-20250302214608054](images/JavaScript.assets/image-20250302214608054.png)

代码

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>js入门</title>
</head>
<body>

    <p id="p1">11111</p>
    <script>
        document.getElementById("p1").innerText="3333"
    </script>
</body>
</html>
```

## 变量与数据类型

变量声明

* let

```js
let 变量名 = 值;

let a = 10;
a  = 200;
```

let 声明的变量可以多次被赋值

* const

```html
const b =  100;
b = 500; // error  不能再次赋值
```

![image-20250302215837583](images/JavaScript.assets/image-20250302215837583.png)

```javascript
const c = [1,2,3]
c[2] = 4  // 可以赋值，常量就是地址不能边
```

![image-20250302220121235](images/JavaScript.assets/image-20250302220121235.png)

* var

var 可以被多次赋值，能用let 就用let。

基本类型

* undefined 和null

**函数没有返回值** 就是 undefined,或者打印**对象**不存在的属性，或者声明的变量没有赋值，要是打印不存在的变量就报错

![image-20250302220746933](images/JavaScript.assets/image-20250302220746933.png)

undefine 都是js才产生的，null是我们自己设置的（后端响应）。



3）string

```html
<a href="https://www.baidu.com">百度</a>
```

用java和 JavaScript 串来表示上述字符串

java

```java
String s1 = "<a href=\"https://www.baidu.com\">百度</a>"   //转义
  String s2 = """
        String s1 = "<a href="https://www.baidu.com">百度</a>"
        """; // 8以上的才支持
```

![image-20250302221824121](images/JavaScript.assets/image-20250302221824121.png)



JavaScript

```javascript
let s1 = '<a href="https://www.baidu.com">百度</a>'

let s3 =`<a href="https://www.baidu.com">百度</a>`
```

![image-20250302222124500](images/JavaScript.assets/image-20250302222124500.png)



模板字符串

需求拼接 URI的请求参数

```txt
/test?name=li&age=20
/test?name=liu&age=21
```

传统方法拼

```javascript
let name = "li"
let age = 20
let uri = "/test?name=" +name + "&age=" +age
```

![image-20250302222616957](images/JavaScript.assets/image-20250302222616957.png)

模板字符串拼接

```javascript
let name = "li"
let age = 20

let uri = `/test?name=${name}&age=${age}`
```

![image-20250302222812258](images/JavaScript.assets/image-20250302222812258.png)



## 运算符表达式

## 控制语句

## API

## 模块化

