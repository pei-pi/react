## 虚拟DOM的两种创建方式

### 1.jsx

```jsx
<script type="text/babel">   //因为是jsx，所以此处一定是babel
    const VDOM = <h1 id='title'>Hello,React</h1>    //此处一定不能写引号
    ReactDOM.render(VDOM,document.getElementById("test"))
</script>
```

### 2.原生js

```js
const VDOM = React.createElement('h1',{id:'title'},'Hello,React')
ReactDOM.reader(VDOM,,document.getElementById("test"))
```

若<h1></h1>内要嵌套<span></span>标签

```js
const VDOM = React.createElement('h1',{id:'title'},React.createElement('span',{},'Hello,React'))
```

缺点：操作繁琐

## 关于虚拟DOM和真实DOM

1. 虚拟DOM本质是一个Object对象
2. 虚拟DOM是React内部在用，所以没有真实DOM上那么多的属性
3. 虚拟DOM最终会转化成真实DOM

## jsx语法规则

1. 定义虚拟DOM时，不要写引号
2. 标签中混入JS表达式时要用{}
3. 样式的类名指定不要用class，要用className
4. 内联样式，要用style={{key:value,key:value}}的形式去写
5. 只有一个根标签
6. 标签必须闭合
7. 关于标签首字母
   - 若小写字母开头，则将该标签转为html中同名元素，若html中无同名元素，则报错
   - 若大写字母开头，react会渲染对应的组件，若组件没有定义，则报错

注意：{ }中只能写表达式

###### 区分【js语句（代码）】与【js表达式】

- 表达式：一个表达式会产生一个值，可以放在任何一个需要值的地方（可以使用变量接收值）

  - a
  - a+b
  - demo(1)
  - arr.map( )
  - function test( ){ }

- 语句（代码）

  - if( ){ }
  - for( ){ }
  - switch( ){case:xxxx} 

  

  



​	