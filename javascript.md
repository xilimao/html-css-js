## js：脚本语言
针对静态页面存在 的语言 弱类型语言
使html动起来
## JavaScript
bs：在服务器校验数据
js：先在本地校验一下
导入问题：设置js文件的编码方式
### 数据类型

    数值型：整型和浮点型
    Boolean类型：true false
    字符串类型：
    char类型

### 变量

    先用var声明，之后赋值
    var str;
    str="hello"
    var innt;
    innt = 10;
    document.write(str+"<br/>");

### 运算符
- 算术运算符
- 比较运算符
- 逻辑运算符

### 流程控制语句

    和java类似、只不过变量用var声明
    while
### 语法问

    大小写敏感
    
### 注释

    //单行注释
    /*多行注释
    */
### 类型转换

    praseInt（String）:字符串转换为整形
    parseFloat(String):字符串类型转换为小数
    
### 函数

    //无参数
    function showMessage(){
        
    }
    //有参数 多个参数就排出来 
    function showMessage(a1,a2){
        
    }
    //带返回值的
    funtion tel(){
        return "hello"
    }
### 变量
- 全局
- 局部

### 事件
onload：当页面加载完之后，执行该函数
```
    <body onload="test()">
    <body>
```
onclick:鼠标点击时间
onmouseover:鼠标滑上
onmouseout：鼠标离开
onchanger:针对select下拉菜单的
onfocus：得到焦点
onblur:失去焦点
onsubmit:表单提交的时候用
### 计算器案例
    ==双引号里边有双引号，则里边的变成单引号（依然表示字符串）==
     ==单引号里边有单引号，则里边的变成双引号（依然表示char）==
    var n1 = document.getElementById("n1").value;获取数据
  - 动态绑定
       
        给按钮绑定函数， 
    
#### Dom对象模型
- alert:提示信息
- 
- windows对象:
    - 属性：
        
        status
        screen
        location
        history
        document
    - 方法
        
        alert（）


        open
    - 使用windows对象:
        
        windows.open("打开窗口的url","窗口名,"窗口特征")
    - Dialog:
        window.returnValue="大苏打"回传值 
        var 
        window.returnValue=回传值
        火狐的调试工具FireBug
        showModaDialog:可以进行回传值；（goole不支持）
        1. 打开子页面时，接受页面的回传值;（可以为对象）
        2. 子页面关闭时必须回传
        
    - Date对象做时钟显示
        var mydate = new Date();
        var year = mydate.getFullYear();
        var date = mydate.getDate();
        document.getElemenById("mydatediv").innerHTML = str;
        setTimeout("getNowTime()",1000);
    
    在body中使用onload()

    - history 和 location对象
        history.go(-1);返回前个页面
        history.back();
        history.go(-2);一下返回前前个页面
    
        location.href("../DialogDemo.html")；实现页面的跳转
        location.reload();页面重新加载
==var getName=fuction(){};==
句柄

#### Dcoment 对象
- document.getElementById（"btn"）;根据对象id获取的是一个对象;
- document.getElementByName（"username"）[0];根据对象name的属性的值，获取的是一个数组对象;
- document.getElementByClassName("")[0];
- document.getElementByTagName("")[1];
- 案例：滚动的广告
- 案例：全选与全不选
- 菜单的二级联动
#### 数组的问题:
- 数组声明
        
        var array = new Array();
        array[] = "";
        var array = new Array("xx","ww","zz");
    - 数组的遍历
        for() 




    


