# 复习：
- html： 标签元素、form表单、框架
- Css:渲染页面，与html的隔离
- 

### 美工
- 效果图---> 切图---> 
- 图片+html+css 组成静态网页
- javaWeb+mysql+jdbc
- 


==浏览器兼容问题==
### HTML标签
1. 工具
    - webstorm
        - 字体设置
        - 风格——背景
        - 快捷键
        
2. 浏览器
    - goole ie 火狐
3. 文件的后缀
    .html  .htm

    网页中的注释:
    
4. 标签是一组闭合的标签
5. head部分：
    定义网页的特点 ：
        
    meta标签、title标签

    刷新之类的
    
6.body部分：
- bgcolor  背景色 
- background 背景图

7.标题
- ==注意标签的闭合==
- h1 align = center h1   几号标题 和 排列
- P 代表段落
- br/  代表换行
- $nbsp; 代表一个空格
- pre 预格式化  即代码里的什么格式 显示就什么格式 保留空格换行符等
- b 代表加粗
- u 下划线
- sup 上标  /sup 下标 
- 列表
    1. 无序列表 li  前边带点
    2. 有序列表 ul   前边带数字
- font face = “隶书” size = "5" 改字体
- img src="路径"  可以设置宽度和高度 width = 20 hight = 20  align = ""  设置方位
 

==middle 和top bottom一起使用==

==center 和left right 一起使用==

8. 图片 相对路径 绝对路径
-  根据网页的位置 找父亲或者兄弟或者儿子
    - ../ 代表返回上一级 即进入父亲  
- 直接写盘的路径
- 
9.特殊字符：
- @gt  是 >
- @lt     <
- @copy   ©

10. 超级链接
-  a href = “”
- 锚记
    - a name = “sdsd” 
    - a href = "#sdsd" 
11. 走马灯 marque   
 - scrolldelly  滚动延时时间
 - direction   方向
 

### 12.table

```
<table border = "1" //设置边框 width="900" align = "center" > 
    <tr>  //代表一行
        <th>学号 <th> //表头
        <th>学号 <th>
        <th>学号 <th>
        <th>学号 <th>
    <tr>
    <tr>
        <td>学号 <th> //数据列
        <td>学号 <th>
        <td>学号 <th>
        <td>学号 <th>
    <tr>
<table>
```
- td与th的区别 ： th一般表示表头，默认加粗居中
- cellspacing : 两条边框的间距
- cellpadding : 内容与边框的间距
- caption : 表的名字
- thad 表头标签
- tbody 主体标签
- 合并单元格
    - ==都是在td 里边写== 
    - 合并列
        - colspan = "n个" 写在标签里
        - respan = "n个" 往下延伸覆盖的行数

    - 合并行 
### 13.form表单
- action：表单提交的url地址
- method：提交方式
    - get：请求参数放在uril后面，对于请求参数的数据量有限制
    - post：请求参数放在包头，对数据量没有限制

    ==value 设置默认回显==
```
 <input tyoe = "text" name = "username" size =  value = "admin">
```

- 单选按钮
- 多行文本域 textarea，标签中间禁止加空格或者换行符 rows高度 cols宽度  注意数据的回显
-下拉菜单  
```
<select name = "  ">
    <option value="sd" multiple = "multiple">山东省</option>
```
    - multiple 是多选 不加的话是单选
    - opyion 后 加select 就默认显示这一项
- 按钮 submit 附带提交功能 reset 重置功能 button 只是button 没有提交


- hidden 隐参 向后台传递数据但不会显示在界面
- disable = disable:销毁此控件，次文本框的值不会向后台传递
- readonly = readonly 改成只读属性，不能更改，但是可以向后台传递  

- file 用来文件上传 


### 14.frameset框架
-  需要放在body外面
-  framest布局
    -  rows表示上下结构，rows="100,*,100" 分为三部分高度分别为100 剩余 100.
    -  frameborder=“no” 表示没有边框
    -  frame 表示具体的某一个页面
    
            如果要在某一区域内显示网页内容，则给该区域设置name属性，  并且指定a标签的targ=该name的值


### CSS样式表（一些风格）
- #### CSS选择器  选择某段内容进行修饰
    ==id>类别>标签>复合  越近越生效==
    - 标签选择器
        
        选中html中的某段代码进行修饰 使用标签进行选择
    - 类别选择器  使用.表示，选中一类事物。
    - id选择器
    ```
    <style type="text/css">
    #id{
       color: blue; 
    }
    </style>
    ```
    - 复合选择器 
        - 交集选择器 
        ```
        div.myclass{
            color: red;
        }
        ```
        - 并集选择器    
        ```
        div,p{
            color: red;
        }
        ```
        - 后代选择器（）
        ```
        div p.myclass{
            color: red;
        }
        ```
- #### 字体样式设置
          font - family: 对应的写法 字体样式
          font - size : 20px   大小
          color: #ddfdfd
          font - style: italic  斜体之类的
          font-weight: bold  字体加粗
          text - decoration: xxx 给字体加线
          letter-spacing:20px  间距
          text-align  对齐方式
          text-transform: 设置大小写方式
          vertical-align: xx 上下标
          简写: font: 50px LiSu italic 
- #### 样式使用方式
    ==优先级：行列样式>内嵌式>外部引入==
    - 内嵌式 : 一般直运用于该界面
    - 外联式 : 外联样式表
    - 行列样式 : 直接写在标签内
- #### 超级链接
    -  a:link 未被点击时样式
    -  a:hover 鼠标悬停的样式
    -  a:visted 点击后的样式
- #### 表格样式
    - border:solid 1px #sdsdsd 简写形式 
    - border-collapse: collapse 内外边框合并
    - 隔行变色  奇数偶数行分别设两个class名 然后设置样式
- #### 盒子模型
    -  margin - top left right bottom 盒子外部
        - margin: 10px 10px 20px 20px 简写 
    -  padding - t l r b  盒子内部
    -  
    -  颜色设置
    -  边线样式
    -  边线粗细
    -  4条边框分别设置
- ==*代表选中所有的组建 包含body==
- #### div定位
    -  默认div宽度：屏幕的宽度 高度默认为0随着内容扩充
    -  float浮动
        - left 向左浮动
        - right 
        - none 默认值
        - inherit 从父元素继承float属性
        - 图片环绕
        - 首字下沉
        - 防止缩放图片会改变位置 给父容器设置固定长度
    - position定位
        - relative(相对定位) :
        - 相对于自身在标准流中的原始位置
        - 其他div还以为他还在原来的标准流的位置
                top :
                left
                buttom
                right
        - z-index:如果有多层 正数在上面 0在中间 负数在下面
    - 若次容器的父及容器未设置定位方式，则次容器以浏览器作为标准，若设置了，则以父容器为标准。
    -  
        如果定位方式视为绝对定位，此元素将脱离标准流
    - fixed 制作广告语：
        - 以浏览器作为标准，设置浏览器的位置 :left right top muttom
- #### 导航
    - 背景色做导航
            
            无序列表 
        - 设置成横向的

    - 背景图
    - 元素的分类:
        
            - 块级元素：默认占据一行
            - 行级元素：默认沿着一行排
            ==可以通过调属性==

        display：block ：本来是横的变成块级元素，然后就扩充容器 
        横的变竖的，竖向变横向
- #### css+div布局
