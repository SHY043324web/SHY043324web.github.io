# Vue.js - Day1

## 课程安排
+ 从Node阶段开始，就已经进入前端中高级的学习过程；
+ React， Vue， Angular(三大框架一大抄)
+ 前3天 主要学习 Vue 的基础语法（打基础的）
+ 第4天 ~ 第 5 天 ，学习前端的自动化构建工具 Webpack(能够自己手写配置基本的配置文件，搭建项目的结构)
+ 后3天 - Vue 项目


## 框架和库的区别
+ 小而巧的是库； 大而全的是框架
 + 框架：是一套完整的解决方案；对项目的侵入性较大，项目如果需要更换框架，则需要重新架构整个项目。
  - express 就是一个Node框架
 + 库（插件）：提供某一个小功能，对项目的侵入性较小，如果某个库无法完成某些需求，可以很容易切换到其它库实现需求。
  -  Bootstrap Jquery -> Zepto
  - MUI 严格来说是框架（因为 MUI 可以 做 手机App开发）


## 为什么要学习流行框架
+ 企业角度：
  - 企业中需要使用流行框架来提高项目的开发效率；（本质目的：节约成本）
  - 原生JS + HTML（Table 布局）
  - Jquery 诞生了 + Ajax
  - Art-template
  - React ， Angular ， Vue
+ 个人角度：
 - 有需求就有买卖
 - 为了能有一个比较不错的收入
 - 提高竞争力和对技术的把握程度
 - 大家学习的不仅仅是框架


### 什么是Vue.js
+ Vue.js 是前端的**主流框架之一**，和Angular.js、React.js 一起，并成为前端三大主流框架！
+ Vue.js 是一套构建用户界面的框架，**只关注视图（页面）层**，它不仅易于上手，还便于与第三方库或既有项目整合。
+ 前端的主要工作是什么？
 - 1. 根据美工的效果图，绘制静态页面
    + Table 表格布局 + Font 标签 + 图片
    + DIv + CSS 
    + HTML5 + CSS3
    + Bootstrap
 - 2. 调用后端提供的API接口，填充页面中的数据
    + 原生JS获取数据，自己使用原生JS拼接 字符串，填充页面数据
    + Jquery 发起Ajax，填充页面数据
    + Jquery + art-template + ajax
    + Vue + Ajax 来填充页面数据和 渲染页面模板


## Node（后端）中的 MVC 与 前端中的 MVVM 之间的区别（了解内容）
 + MVC 主要是后端的分层开发思想；
 + MVVM是前端页面的分层开发思想，主要关注于 **视图层** 分离，也就是说：MVVM把前端的视图层，分为了 三部分 Model, View ,  ViewModel
 + 为什么有了MVC还要有MVVM


## Vue.js 基本代码 和 MVVM 之间的对应关系


## 什么是Vue中的指令
定义： Vue 中，通过一些特殊的语法，扩展了 HTML 的能力；将来当 创建 Vue 实例的时候，Vue 会把 这些指令 都进行解析，从而，根据不同的指令，去渲染不同的结果；


## Vue指令之 `插值表达式`
1. 基本使用演示
2. 在插值表达式中 使用简单的语句
## Vue指令之 `v-cloak`
1. 解决的问题
插值表达式有闪烁的问题（v-cloak 指令来解决闪烁问题）
2. 应用场景
当 网络比较卡的时候，我们可以为 最外层的 元素，添加 v-cloak ，防止用户看到 插值表达式


## Vue指令之 `v-text`
1. 基本使用
 在 元素的属性节点上，添加`v-text`指令
2. 在`v-text`中 使用简单的语句
3. 和 插值表达式的两点区别和各自的应用场景
 + 插值表达式只是一个占位符，但是，v-text会把内容区域之前的内容覆盖掉
 + 插值表达式有闪烁问题，但是，v-text不存在闪烁问题
 + 插值表达式适合在 前后追加一个元素的内容；
 + 如果 想要防止插值表达式闪烁问题，同时，没有其它内容，推荐使用 v-text
## Vue指令之 `v-html`
1. 基本使用
2. 应用场景
 + 当 服务器返回的数据中，包含的HTML的标签，此时，这些标签只能使用 v-html 来渲染；



## Vue指令之 `v-bind`
1. 基本使用
 + v-bind 是为 html 属性节点绑定数据的
2. 应用场景
 + 当 HTML 元素上，某些 属性的数据，需要从 Vue 身上的数据来填充的时候，大家需要把 对应的属性前面，添加 v-bind: 指令来修饰
## Vue指令之 `v-on`
1. 基本使用： 
 + `<input type="button" value="按钮" v-on:click="事件处理函数名" />`
 + `<input type="button" value="按钮" @click="事件处理函数名" />`
 + v-on 是为 HTML 元素，绑定 处理事件的；


## 上午内容总结
1. MVC 和 MVVM 概念
2. Vue中基本的代码结构和MVVM的对应关系
 + 配置对象中： el   data  methods
3. 指令：
 + {{  }}
 + v-text
 + v-cloak
 + v-html
 + v-bind:    简写   : 
 + v-on:       简写  @


## 【案例】跑马灯效果


## Vue指令之 `v-model` 实现 双向数据绑定
1. 基本使用（案例：自动在页面输出文本框中字符串的长度）
2. 应用场景
 + 应用给表单元素


## 【案例】简易计算器案例


## 在Vue中使用class样式
1. 类名数组
2. 类名数组中使用**三元表达式**，按需为元素添加某些类名
3. 应用场景（案例：网页开关灯 等类名切换效果）


## Vue指令之`v-for`和`key`属性
1. 迭代数组
 + 普通数组（一般般）
 + 对象数组（用的最多）
  `(item, i) in objList`
2. 迭代对象中的属性（用的不多）
3. 迭代数字（几乎没人用）

> 2.2.0+ 的版本里，**当在组件中使用** v-for 时，key 现在是必须的。

+ 当 Vue.js 用 v-for 正在更新已渲染过的元素列表时，它默认用 “**就地复用**” 策略。如果数据项的顺序被改变，Vue将**不是移动 DOM 元素来匹配数据项的顺序**， 而是**简单复用此处每个元素**，并且确保它在特定索引下显示已被渲染过的每个元素。

+ 为了给 Vue 一个提示，**以便它能跟踪每个节点的身份，从而重用和重新排序现有元素**，你需要为每项提供一个唯一 key 属性。

## Vue指令之`v-if`和`v-show`
+ v-if 和 v-show 的作用，都是切换界面上元素的显示或隐藏的；

> 一般来说，v-if 有更高的**切换消耗** 而  v-show 有更高的**初始渲染消耗**。

> 因此，如果需要频繁切换 v-show 较好，如果在运行时条件不大可能改变 v-if 较好。
+ 根据应用场景区分：
> 举例：袜子要不要洗的问题


## 回顾今天主要知识点：
1. MVC 和 MVVM  的区别
2. Vue基本的代码和 MVVM 的对应关系
3. 插值表达式 （Mustache）    {{  }}      v-cloak    1. 为元素添加 v-cloak 属性，2. 添加样式，属性选择器  [v-cloak]{ display: none; }
4. v-text
5. v-html
6. v-bind: 为元素的属性绑定数据   缩写 :
7. v-on:    为元素绑定 Vue 事件处理函数   v-on:click="show()"    缩写为 @
8. v-model  在vue指令中，唯一实现了双向数据绑定的指令  只能应用给 表单元素（进一步解放了程序员的双手）
9. v-bind:class="['color', flag ? 'thin': '']"  按需为元素添加某些类样式
10. v-for 指令     <li v-for="(item, i) in list" :key="item.id"></li>
 + :key 的值 只接受 string 或者 number
 + :key 的值要具有唯一性
 + 今后，一定要把 :key 带上
11. v-if 和 v-show


## 品牌管理案例
### 添加新品牌
### 删除品牌
### 根据条件筛选品牌
1. 1.x 版本中的filterBy指令，在2.x中已经被废除：
[filterBy - 指令](https://v1-cn.vuejs.org/api/#filterBy)
```
<tr v-for="item in list | filterBy searchName in 'name'">
  <td>{{item.id}}</td>
  <td>{{item.name}}</td>
  <td>{{item.ctime}}</td>
  <td>
    <a href="#" @click.prevent="del(item.id)">删除</a>
  </td>
</tr>
```
2. 在2.x版本中[手动实现筛选的方式](https://cn.vuejs.org/v2/guide/list.html#显示过滤-排序结果)：
+ 筛选框绑定到 VM 实例中的 `searchName` 属性：
```
<hr> 输入筛选名称：
<input type="text" v-model="searchName">
```
+ 在使用 `v-for` 指令循环每一行数据的时候，不再直接 `item in list`，而是 `in` 一个 过滤的methods 方法，同时，把过滤条件`searchName`传递进去：
```
<tbody>
      <tr v-for="item in search(searchName)">
        <td>{{item.id}}</td>
        <td>{{item.name}}</td>
        <td>{{item.ctime}}</td>
        <td>
          <a href="#" @click.prevent="del(item.id)">删除</a>
        </td>
      </tr>
    </tbody>
```
+ `search` 过滤方法中，使用 数组的 `filter` 方法进行过滤：
```
search(name) {
  return this.list.filter(x => {
    return x.name.indexOf(name) != -1;
  });
}
```


## 过滤器
概念：Vue.js 允许自定义过滤器，**可被用作一些常见的文本格式化**。过滤器可以用在两个地方：**mustache 插值和 v-bind 表达式**。过滤器应该被添加在 JavaScript 表达式的尾部，由“管道”符指示；

### 全局过滤器
### 私有过滤器

> 使用ES6中的字符串新方法 String.prototype.padStart(maxLength, fillString='') 或 String.prototype.padEnd(maxLength, fillString='')来填充字符串；

> 注意过滤器查找顺序问题：


## Vue调试工具`vue-devtools`的安装步骤和使用
[Vue.js devtools - 翻墙安装方式 - 推荐](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd?hl=zh-CN)


## 相关文章
1. [vue.js 1.x 文档](https://v1-cn.vuejs.org/)
2. [vue.js 2.x 文档](https://cn.vuejs.org/)
3. [String.prototype.padStart(maxLength, fillString)](http://www.css88.com/archives/7715)
4. [js 里面的键盘事件对应的键码](http://www.cnblogs.com/wuhua1/p/6686237.html)
5. [Vue.js双向绑定的实现原理](http://www.cnblogs.com/kidney/p/6052935.html)