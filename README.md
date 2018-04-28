# learning-of-vue
This is a note to record my experience of vue studing

#关于入口文件的配置

一、vue-router 实例化时哪些是一定要配置的？
1、初始页面一定要配置；
2、所有页面都需要去配置
3、如果需要配置的路由太多，可以将其分离成一个单独的js文件

二、子路由是如何配置的，以及它的主要应用场景是什么？
1、配置当前路由时，添加一个children参数，对应的参数值和父页面一样配置路径和组件
2、在存在子路由的父页面需要有<router-view>标签，用于存放子路由页面的容器
3、完成路由切换可以使用编程式导航和<router-link>标签(声明式导航)两种方式
    ##编程式导航与标签导航的区别和优缺点各是什么？ router.push、router.replace 、router.go 与 <router-link>
    #A#:编程式导航更加灵活，只需要在指定标签上绑定click事件即可，参数传递也更加灵活
    #B#:能够在浏览器里不保留路由历史，和多级跳转
    
三、为什么在组件中this代表的是VUE实例？


四、如何在vue项目中添加全局的实例方法
   1、Vue.prototype.fn = function(){}  ;添加fn方法
