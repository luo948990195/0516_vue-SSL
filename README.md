# vue-5

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

 ## 项目源码目录设计 
   api  与后台交互模块文件夹
   common  通用资源文件夹  img/fonts/
   components  非路由组件文件夹
   filters  自定义过滤器模块文件夹
   mock 模拟数据接口文件
   pages 路由组件文件夹 
   router 路由器文件夹 
   store vuex相关模块文件夹

##  引入static/css/reset.css  初始化CSS

## flex布局 
  flex-direction: row | row-reverse | column | column-reverse; 决定主轴的方向
  flex-wrap: nowrap (不换行)| wrap (换行)| wrap-reverse(第一行在下方);
    justify-content: flex-start | flex-end | center | space-between | space-around; 项目在主轴上的对齐方式
    align-items: flex-start | flex-end | center | baseline | stretch; 项目在交叉轴上如何对齐
    align-content: flex-start | flex-end | center | space-between | space-around | stretch;多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用
    order属性定义项目的排列顺序。数值越小，排列越靠前，默认为0。
    align-self属性允许单个项目有与其他项目不一样的对齐方式
    flex-shrink:1  当父元素的宽度小于子元素宽度之和时,会按照一定的比例进行收缩