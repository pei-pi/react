# React全家桶

## 一、React基础

#### 1.React是什么？

用于构建用户界面的JavaScript库（操作DOM呈现页面）

#### 2.为什么要用React

1. 原生JavaScript操作DOM繁琐、效率低（DOM-API操作UI）
2. 使用JavaScript直接操作DOM，浏览器会进行大量的重绘重排
3. 原生JavaScript没有组件化编码方案，代码复用率低

#### 3.React的特点

1. 采用组件化模式、声明式编码，提高开发效率及组件复用率
2. 在React Native中可以使用React语法进行移动端开发
3. 使用虚拟DOM+优秀的Diffing算法，尽量减少与真实DOM的交互

#### 4.创建组件的两种方式

1. 函数式组件（适用于【简单组件】的定义）
2. 类式组件（适用于【复杂组件】的定义）如果组件有状态，则是复杂组件

#### 5.组件实例三大属性

前提：类式定义的组件

##### 1.state

- state是组件对象最重要的属性，值是对象（可以包含多个key-value的组合）

- 组件被称为“状态机”，通过更新组件的state来更新对应的页面显示（重新渲染组件）

- 组件中render方法中的this为组件实例对象

- 组件自定义的方法中this为undefined，如何解决？

  - 强制绑定this:通过函数对象的bind()

  - 箭头函数

- 状态数据，不能直接更改或更新

##### 2.props



## 二、React-Router路由



## 三、PubSub消息管理

## 四、Redux集中式状态管理

## 五、Ant-Design  UI组件库

