vue
================

Vue发音(view);

* **console的用法** 

        //显示对象的所有属性
        console.dir(对象);
        
        //测试代码的执行效率
        condole.time("test");
        //测试的代码
        condole.endtime("test");

* **安装VueDevTool工具**         

        1、翻墙
        2、https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd
        
        
**1.最简单的例子**

通过此实例学习以下内容

        1、搭建过程
        2、模板语法
        3、理解Vue实例【var vm=new Vue({el:'#app',data:data})】,每一个应用或组件都是一个vue实例或实例的组合。
           当一个Vue实例创建时，它向Vue的响应式系统中加入了数据对象model，且与视图view建立了双向绑定关系。
        4、实例的生命周期https://cn.vuejs.org/images/lifecycle.png.      

* **制作步骤**

        1、下载vue.js
        2、设置nginx
        3、重启nginx

* **代码情况**
        
        请查看ex/ex1.html文件

* **知识点**

        1、双大括号:文本
          例如:{{ message }}
        2、v-once:节点及其子节点一次性绑定
        3、v-html:输出html
        4、v-bind:文本语法"{{}}"不能作用在元素的属性上，如果要绑定在属性上需要使用v-bind
        5、使用模板表达式
        
        6、只用当Vue实例创建时传入的data才会建立绑定，后续在data中增加的属性不会建立绑定关系
        7、在创建实例前执行了Object.freeze(data)可以解除绑定关系，不会响应
        8、调用实例属性或方法
        9、生命周期钩子
        
 **2.指令、计算属性、方法、监听器**
 
 指令是带 v- 前缀的命令，通过此实例学习以下内容
 
         1、指令
         2、带参数的指令,例如:v-bind、v-on
         3、指令缩写    
         4、计算属性,在实际应用中，不要是用过于复杂的表达式，如果表达式比较复杂，则建议使用计算属性
            计算属性,连续使用两次计算属性，如果计算属性关联的变量不发生变化，则调用的是缓存，不会触发计算属性内部的执行
         5、方法
            连续使用两次方法，不论方法关联的变量发不发生变化，都会触发方法内部的执行
         6、监听器   
         
 * **制作步骤**
 
 
 * **代码情况**
         
         请查看ex/ex2.html文件
 
 * **知识点**
 
         1、v-if:控制是否显示        
         2、v-on:监听DOM事件
         3、缩写v-on:'@'
         4、缩写v-bind:':'
         5、计算属性,连续使用两次计算属性，如果计算属性关联的变量不发生变化，则调用的是缓存，不会触发
            计算属性内部的执行
         6、方法,连续使用两次方法，不论方法关联的变量发不发生变化，都会触发方法内部的执行
         7、计算属性的set和get写法
         8、监听器的用法
         