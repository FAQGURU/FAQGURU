## Vue.js

[如何创建一个vuejs实例?](#如何创建一个vuejs实例)

[Vue.js是什么?](#vuejs是什么)

[如何在Vue.js中使用local storage?](#如何在vuejs中使用local-storage)

[如何在Vue.js中创建双向绑定?](#如何在vuejs中创建双向绑定)

[Vue.js的过滤器是什么(一)?](#vuejs的过滤器是什么一)

[组件的props是什么?](#组件的props是什么)

[如何部署一个Vue.js应用?](#如何部署一个vuejs应用)

[Vue.js的组件是什么?](#vuejs的组件是什么)

[什么是Vue.js的指令?列举出其中的一些](#什么是vuejs的指令列举出其中的一些)

[Vue.js的过滤器是什么(二)?](#vuejs的过滤器是什么二)

[列举Vue.js的一些特性](#列举vuejs的一些特性)

[如何在Vue.js中重定向到其他页面?](#如何在vuejs中重定向到其他页面)

[在Vue.js中可以通过传参来计算属性吗?](#在vuejs中可以通过传参来计算属性吗)

[解释一下Vue.js应用组成的基本逻辑](#解释一下vuejs应用组成的基本逻辑)

[Vue.js的优点以及缺点有哪些?](#vuejs的优点以及缺点有哪些)

[解释一下单向数据流跟双向数据绑定的不同点?](#解释一下单向数据流跟双向数据绑定的不同点)

[如何在Vue.js中获取query的参数?](#如何在vuejs中获取query的参数)

[列举在Vue.js里面可以使用的指令类型](#列举在vuejs里面可以使用的指令类型)

[如何在Vue.js中使用循环?](#如何在vuejs中使用循环)

[v-bind跟v-model的区别是什么? 举一些例子。](#v-bind跟v-model的区别是什么-举一些例子)

[如何在父组件调用子组件的函数?](#如何在父组件调用子组件的函数)

[列举Vue.js的一些好处](#列举vuejs的一些好处)

[如何往过滤器传参?](#如何往过滤器传参)

[如何避免Vue.js的内容跳动?](#如何避免vuejs的内容跳动)

[如何在Vue.js中使用gulp?](#如何在vuejs中使用gulp)

[可以让Vue.js重新加载或者重新渲染吗?](#可以让vuejs重新加载或者重新渲染吗)

[如何把你的样式绑定到Vue.js上?](#如何把你的样式绑定到vuejs上)

[可以监听组件里面props的变化吗?](#可以监听组件里面props的变化吗)

[可以实现监听组件里面props的变化吗?](#可以实现监听组件里面props的变化吗)

[Vue.js里面跟Angular的Service等价的是什么?](#vuejs里面跟angular的service等价的是什么)

[Vuex是什么?](#vuex是什么)

[如何使用Vue.js实现无论在什么时候，都要把用户类型的值保存到data变量里面的功能?](#如何使用vuejs实现无论在什么时候都要把用户类型的值保存到data变量里面的功能)

[如何实现简易的Vue.js路由(不使用第三方库)?](#如何实现简易的vuejs路由不使用第三方库)

[列举一些Vue.js app里面组件通信的方式](#列举一些vuejs-app里面组件通信的方式)

[如何在Vue.js监听一个数组长度的变化?](#如何在vuejs监听一个数组长度的变化)

[我们为什么需要Vue.js的混入(mixins)?](#我们为什么需要vuejs的混入mixins)

[创建一个可以让整个Vue.js应用访问的常量的最佳方式是什么?](#创建一个可以让整个vuejs应用访问的常量的最佳方式是什么)

[在Vue.js中method跟computed value有什么区别?](#在vuejs中method跟computed-value有什么区别)

[在Vue.js 2.0中兄弟组件间通信的正确方式是什么?](#在vuejs-20中兄弟组件间通信的正确方式是什么)

[如何在Vue.js切换class?](#如何在vuejs切换class)



### 如何创建一个vuejs实例?

每一个Vue应用都是从创建一个新的Vue实例函数开始的:

```js
var vm = new Vue({
  // 选项
})
```

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### Vue.js是什么?

**Vue js**是用于创建动态界面的JavaScriptj脚本。学习Vue.js是非常简单的。为了能够让Vue.js运行，你只需要在网站上添加少量动态功能。在项目中使用Vue.js不需要添加其他的东西，你只需要把Vue.js库添加到项目中。

###### 来源

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js中使用local storage?

你只需根据下面代码执行:

```js
localStorage.setItem('YourItem', response.data)
localStorage.getItem('YourItem')
localStorage.removeItem('YourItem')
```

###### 来源

* https://stackoverflow.com/questions/41425889/vue-js-how-to-use-localstorage-with-vue-js

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js中创建双向绑定?

`v-model`指令用于在Vue.js中创建双向绑定。双向数据绑定就是把data或者model绑定到DOM上，然后DOM又绑定在model上。

你可以从下面的例子来了解双向绑定的实现。

```html
<div id="app">
  {{message}}
  <input v-model="message">
</div>
<script type="text/javascript">
  var message = 'Vue.js is rad';
  new Vue({ el: '#app', data: { message } });
</script>
```

###### 来源

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### Vue.js的过滤器是什么(一)?

Vue.js的过滤器是用于转换要渲染在浏览器的内容。

Vue.js过滤器的本质是一个函数，它需要接收一个值并处理它，然后返回一个处理过后的值。它用管道符号(|)表示，可以接收一个或者多个参数。

```html
<element directive="expression | filterId \[args...\]"></element>
```

###### 来源

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### 组件的props是什么?

每一个组件都有它自己的作用域。这意味着你不能(和不应该)在子组件模板(template)上直接引用父组件的data。可以使用**props**来把data传递给子组件。props是必须注册在组件上的自定义属性。当把一个值传入prop属性(attribute)时，它变成了组件实例上的属性(property)。

```js
Vue.component('blog-post', {
  // camelCase in JavaScript
  props: ['postTitle'],
  template: '<h3>{{ postTitle }}</h3>'
})
```

###### 来源

* https://vuejs.org/v2/guide/components-props.html#ad

[[↑] 返回顶部](#vuejs)
### 如何部署一个Vue.js应用?

如果你已经按照以下步骤创建项目:
```sh
vue init webpack myproject
```
Now you can run
```sh
npm run build
```
然后你只需要复制 index.html 和 /dist/ 目录到你网站的root目录即可。

###### 来源

* https://stackoverflow.com/questions/42936588/how-to-deploy-vue-app

[[↑] 返回顶部](#vuejs)
### Vue.js的组件是什么?

**组件(Components)**是Vue.js的一个很强大的特性。Vue的组件使用自定义的元素来扩展基本的HTML元素，把它封装到一段可复用的代码中。

以下步骤是在其他组件里面注册一个Vue组件:

```js
export default {
  el: '#your-element'
  components: {
      'your-component'
  }
}
```

###### 来源

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### 什么是Vue.js的指令?列举出其中的一些

Vue.js中的指令要比Angular中的简单。Vue.js的指令提供了一个新的属性和标记来扩展HTML。Vue.js有很多内置的指令，为应用提供了扩展的功能。你也可以在Vue.js中编写自定义的指令。

以下是一些常用的Vue.js指令。

*   v-show
*   v-if
*   v-model
*   v-else
*   v-on

###### 来源

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### Vue.js的过滤器是什么(二)?

Vue.js允许你定义**过滤器(filters)**，可被用于格式化普通的文本。过滤器可以在两个地方使用: 双括号插值和v-bind表达式(后者从2.1.0+的版本开始支持)。过滤器应该写在JavaScript表达式尾部，用“管道“符号表示:

```html
<!-- in mustaches -->
{{ message | capitalize }}

<!-- in v-bind -->
<div v-bind:id="rawId | formatId"></div>
```

###### 来源

* https://vuejs.org/v2/guide/filters.html

[[↑] 返回顶部](#vuejs)
### 列举Vue.js的一些特性

Vue.js有以下的特性:

*   模板语法(Templates)
*   响应式(Reactivity)
*   组件化(Components)
*   过渡效果(Transitions)
*   路由(Routing)

###### 路由

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js中重定向到其他页面?

如果你在使用`vue-router`，你可以使用`router.go(path)`来导航到其他指定的路由。在组件里面可以使用`this.$router`、`router.go()`访问路由，这是在Vue.js2.0改变的。你可以使用`router.push({ name: "yourroutename" })`或者使用`router.push("yourroutename")`来实现重定向。

[[↑] 返回顶部](#vuejs)
### 在Vue.js中可以通过传参来计算属性吗?

你可以使用 _method_ 或者 _computed function_。

使用method:

```js
<span>{{ fullName('Hi') }}</span>

methods: {
  fullName(salut) {
      return `${salut} ${this.firstName} ${this.lastName}`
  }
}
```

使用计算属性:

```js
computed: { 
	fullName() {
		return salut => `${salut} ${this.firstName} ${this.lastName}`
  }
}
```

[[↑] 返回顶部](#vuejs)
### 解释一下Vue.js应用组成的基本逻辑

一个**Vue.js应用**包含一个使用 new Vue 来创建根 Vue 实例，以及可选的嵌套的、可复用的组件树组成.举个例子，一个todo app的组件树结构可以是这样的:

```sh
根实例
└─ TodoList
   ├─ TodoItem
   │  ├─ DeleteTodoButton
   │  └─ EditTodoButton
   └─ TodoListFooter
      ├─ ClearTodosButton
      └─ TodoListStatistics
```
所有Vue组件都是Vue实例。

###### 来源

* https://vuejs.org/v2/guide/instance.html

[[↑] 返回顶部](#vuejs)
### Vue.js的优点以及缺点有哪些?

**Vue.js的优点**
- 使应用程序和接口的开发变得简单
- 像Angular.js一样支持双向通信
- 有控制状态的能力
- 自然的思考过程

**Vue.js的缺点**
- 使用范围受限
- 单独的开发者
- 开发者社区小

[[↑] 返回顶部](#vuejs)
### 解释一下单向数据流跟双向数据绑定的不同点?

在单向数据流中，当数据模型发生改变的时候，view(UI)部分并不会随之改变，我们需要编写代码使得数据模型每次发生改变的时候来让它更新。而在Vue.js中，**v-bind**被用于实现单向数据流或者绑定。

在双向数据绑定中，当数据模型发生改变的时候，view(UI)会自动更新。在Vue.js中使用**v-model**指令来实现双向数据绑定。

###### 来源

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js中获取query的参数?

你可以在组件里面使用`$route`对象来暴露我们需要的参数。

```js    
// 在组件里面
console.log(this.$route.query.test)
```

###### 来源

* https://stackoverflow.com/questions/35914069/vue-js-query-parameters

[[↑] 返回顶部](#vuejs)
### 列举在Vue.js里面可以使用的指令类型

在Vue.js中可以使用下列类型的指令:

*   普通指令
*   字面量指令
*   空指令
*   自定义指令

###### 来源

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js中使用循环?

你可以在template里面使用这种方法:

```html
<b-menu v-for="menu in menu_items" v-bind:key="menu.label">
    <label>{{ menu.label }}</label>
    <b-menu-list v-for="item in menu.items" v-bind:key="item">
        <b-menu-item> {{ item.message }}</b-menu-item>
    </b-menu-list>
</b-menu>
```

###### 来源

* https://stackoverflow.com/questions/42260233/vue-js-difference-between-v-model-and-v-bind/44678583

[[↑] 返回顶部](#vuejs)
### v-bind跟v-model的区别是什么? 举一些例子。

`v-model`是**表单输入的双向数据绑定**。它结合了`v-bind`(把**js值**存到一个标记里面)跟`v-on:input`(**更新js值**)。

仔细思考下面代码:
```html
<input v-model="something">
```
它只是以下代码的语法糖:
```html
<input
   v-bind:value="something"
   v-on:input="something = $event.target.value"
>
```

`v-model`在基本的HTML input类型标签(text，textarea，number，radio，checkbox，select)下生效。假如你的数据模型把日期存储为ISO 字符串 (`yyyy-mm-dd`)，可以在`input type=data`下使用`v-model`。

###### 来源

* https://stackoverflow.com/questions/42260233/vue-js-difference-between-v-model-and-v-bind/44678583

[[↑] 返回顶部](#vuejs)
### 如何在父组件调用子组件的函数?

在父组件(child-component)中使用`$refs`添加一个ref来直接调用子组件的方法。

Html:
```html
<div id="app">
  <child-component ref="childComponent"></child-component>
  <button @click="click">Click</button>  
</div>
```
Javascript:
```js
var ChildComponent = {
  template: '<div>{{value}}</div>',
  data: function () {
    return {
      value: 0
    };
  },
  methods: {
    setValue: function(value) {
        this.value = value;
    }
  }
}

new Vue({
  el: '#app',
  components: {
    'child-component': ChildComponent
  },
  methods: {
    click: function() {
        this.$refs.childComponent.setValue(2.0);
    }
  }
})
```

###### 来源

* https://stackoverflow.com/questions/42632711/how-to-call-function-on-child-component-on-parent-events

[[↑] Back to top](#vuejs)
### 列举Vue.js的一些好处

* 允许使用HTML。这意味着Vue.js跟Angular有很多相似的特征，可以使用不同的组件进行来优化HTML代码块。
* 详细的文档。Vue.js拥有一个非常详细的文档，使得开发者的学习曲线更平缓、更快速的学习，仅使用简单的HTML和JavaScript知识就可以开发出一个应用程序。
* 平滑过渡。由于Vue.js在设计和架构上跟Angular和React很相似，它给开发者提供了一个从其他框架转到Vue.js的快速切换周期。
* 高度集成。Vue.js可以创建单页面应用和不同的应用接口。主要是小的交互模块很容易地集成到整个系统里已有的基础设施当中，这个过程不会产生副作用。
* 大型化。Vue.js可以帮助你开发非常大型的可复用的模板，由于它结构简单，你不需要花费很多的时间去开发。
* 体积小。Vue.js的体积只有20KB左右来保持它的速度跟灵活性，对比其他框架，它拥有更好的性能。

###### 来源

* https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] 返回顶部](#vuejs)
### 如何往过滤器传参?

思考以下代码:
```js
filters:{
   currency: function(value, arg1){
     return arg1+value;
}
```
使用方法:
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.5.1/vue.js"></script>
<div id="vue-instance">
  {{123 | currency('$') }}
</div>
```

###### 来源

* https://vuejs.org/v2/guide/filters.html

[[↑] 返回顶部](#vuejs)
### 如何避免Vue.js的内容跳动?

如果你想完全取消客户端首次渲染，唯一的途径是使用**服务端渲染**。所有你的应用初始化的时候发送一个html结构。

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js中使用gulp?

你可以使用`Vueify`，它是一个`browserify`的转换。

```js
gulp.task('browserify', function() {
    return gulp.src('src/js/main.js')
        .pipe(plumber())
        .pipe(browserify({
            debug: !env.p,
            transform: ['vueify']
        }))
        .pipe(gulpif(env.p, uglify()))
        .pipe(gulp.dest('build/js'));
});
```

[[↑] 返回顶部](#vuejs)
### 可以让Vue.js重新加载或者重新渲染吗?

可以的。思考以下代码:
```js
vm.$forceUpdate();
```

###### 来源

* https://stackoverflow.com/questions/32106155/can-you-force-vue-js-to-reload-re-render

[[↑] 返回顶部](#vuejs)
### 你知道Vue.js有哪些不好的地方吗?

* 资源少。Vue.js相对于React或者Angular来说占有较少的市场份额，意味着这个框架的知识分享仍处于起步阶段。
* 灵活性上的风险。有时候，把Vue.js集成到到大项目的时候会出现一些问题，对于可能的解决方案没有相关的经验。

###### 来源

* https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] 返回顶部](#vuejs)
### 如何把你的样式绑定到Vue.js上?

思考以下代码:
```html
<div id="table">
    <div v-for="table in tables">
        <div class="table-div" v-bind:style="{top: table.top + 'px', left: table.left + 'px'}">{{table.name}}</div>
    </div>
</div>
```

###### 来源

* https://stackoverflow.com/questions/45604244/binding-styles-in-vue-js

[[↑] 返回顶部](#vuejs)
### 可以实现监听组件里面props的变化吗?

可以的。你可以使用`watch`来监听props的变化，props变化的时候执行一些代码:

```js
new Vue({
  el: '#app',
  data: {
    text: 'Hello'
  },
  components: {
    'child' : {
      template: `<p>{{ myprop }}</p>`,
      props: ['myprop'],
      watch: { 
      	myprop: function(newVal, oldVal) { // watch it
          console.log('Prop changed: ', newVal, ' | was: ', oldVal)
        }
      }
    }
  }
});
```
在HTML上使用:
```html
<script src="https://unpkg.com/vue/dist/vue.js"></script>

<div id="app">
  <child :myprop="text"></child>
  <button @click="text = 'Another text'">Change text</button>
</div>
```

###### 来源

* https://stackoverflow.com/questions/44584292/vuejs-2-0-how-to-listen-for-props-changes

[[↑] 返回顶部](#vuejs)
### Vue.js里面跟Angular的Service等价的是什么?

有四种方法:

* 无状态service: 使用mixins
* 有状态service: 使用Vuex
* 导出service和导入一段vue的代码
* 任何JavaScript全局对象

###### 资源

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] 返回顶部](#vuejs)
### Vuex是什么?

Vuex是一个为Vue.js应用程序开发的**状态管理模式和库**。它采用集中式存储来管理应用里面所有组件的状态，并以相应的规则来确保状态是以一种可预测的方式发生变化的。Vuex的灵感来自于Flux，Redux跟Elm的架构。

Vuex解决两个问题:
* 多个视图公用一个state。给多层嵌套的组件传递props是非常繁琐的，并且对于兄弟组件之间的传递也是无能为力的。
* 不同视图的行为，改变的是同一个状态。我们通常使用比如直接在父/子组件实例上直接引用或者通过事件来改变，和同步状态的多份拷贝。这些模式都非常脆弱，而且很容易导致代码不可维护。

###### 来源

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] 返回顶部](#vuejs)
### 如何使用Vue.js实现无论在什么时候，都要把用户类型的值保存到data变量里面的功能?

使用`watch`方法监测储存在data的变量的变化，像这样:

```js
watch: {
  input: function () {
    if (isLocalStorage() /* function to detect if localstorage is supported*/) {
      localStorage.setItem('storedData', this.input)
    }
  }
}
```

###### 来源

* https://stackoverflow.com/questions/41425889/vue-js-how-to-use-localstorage-with-vue-js

[[↑] 返回顶部](#vuejs)
### 如何实现简易的Vue.js路由(不使用第三方库)?

如果你只需要非常简单的路由，并且不想引入整一个router库，你可以像下面这样动态地渲染一个页面级别的组件:

```js
const NotFound = { template: '<p>Page not found</p>' }
const Home = { template: '<p>home page</p>' }
const About = { template: '<p>about page</p>' }

const routes = {
  '/': Home,
  '/about': About
}

new Vue({
  el: '#app',
  data: {
    currentRoute: window.location.pathname
  },
  computed: {
    ViewComponent () {
      return routes[this.currentRoute] || NotFound
    }
  },
  render (h) { return h(this.ViewComponent) }
})
```

对于大多数单页面应用来说，推荐使用官方的vue-router库。

###### 来源

* https://vuejs.org/v2/guide/routing.html

[[↑] 返回顶部](#vuejs)
### 列举一些Vue.js app里面组件通信的方式

* **Props** (`props`) - Vue.js里面最简单的父子组件直接通信的方式。主要用于传递与表示逻辑相关的数据，或者限制层次结构的数据集。
* **Refs 和 methods** (`ref`) - 它对于子组件处理父组件的事件似乎不太合乎情理。在子组件上设置ref，然后调用它的方法(methods)就可以实现。
* **Events** (`$emit`和`$on`) - 它是父子组件直接通信最简单的方式。同样，它应该用于表示逻辑。
* **Event bus** (`this.$root.$emit`, `this.$root.$on`) - 当它要往深层嵌套的组件传递props给子组件的时候非常有用，在这两个组件之间几乎没有其他组件需要传递。
* **集中式储存** (_Vuex_) -Vuex是是Vue.js里面一种状态管理方式。它提供了比单纯通过events传递的更多方式，它为整一个应用的通信做好了充分的准备。

###### 来源

* https://stackoverflow.com/questions/38616167/communication-between-sibling-components-in-vuejs-2-0

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js监听一个数组长度的变化?

在创建的vm中使用watch:
```js
var vm = new Vue({
    el: 'body',
    data: {
        items: []
    },
    computed: {
        item_length: function () {
            return this.battle_logs.length;
        }
    },
    watch: {
        items: {
            handler: function () {
                console.log('caught!');
            },
            deep: true
        }
    }
});
```
或者兼容一个计算好的length属性:
```js
vm.$watch('item_length', function(newVal, oldVal) {
    console.log('caught!');
});
```

###### 来源

* https://stackoverflow.com/questions/37041720/vue-js-watch-array-length

[[↑] 返回顶部](#vuejs)
### 我们为什么需要Vue.js的混入(mixins)?

混入(mixins)是一种分发Vue组件中 _可复用的功能_ 的非常灵活的方式。混入对象可以包含任意组件选项。当一个组件使用混入对象时，所有的混入对象选项都会被"混入"该组件本身的选项。

思考以下代码:
```js
// 定义一个混入对象
var myMixin = {
  methods: {
     getProducts () {
         myApi.get('products?id=' + prodId).then(response =>  this.product = response.data)
      }
  }
}

// 定义一个使用混入的组件
var Component = Vue.extend({
  mixins: [myMixin]
})

// 在初始化的时候使用混入的替代方法
new Vue({
  mixins: [myMixin],
  created: function () {
    console.log('other code')
  }
})
```

###### 来源

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] 返回顶部](#vuejs)
### 创建一个可以让整个Vue.js应用访问的常量的最佳方式是什么?

你可以在Vue应用程序范围外定义一个变量，然后在里面使用它。

```js
//const.js
export default {
   c1: 'Constant 1',
   c2: 'Constant 2'
}
```
And:
```js
// component.vue
import const from './const';

export default {
  methods: {
    method() {
      return const.c1;
    }
  }
}
```

###### 来源

* https://stackoverflow.com/questions/46882944/what-is-the-best-way-to-create-a-constant-that-can-be-accessible-from-entire-ap

[[↑] 返回顶部](#vuejs)
### 在Vue.js中method跟computed value有什么区别?

* computed value跟methods很不同，在Vue.js里面，大多数情况下绝对不能互换。
* 对于computed value有一个更贴切的名字叫**计算属性**。你可以把computed value看成一个派生值，当计算该值的一个值发生改变时，它将会自动更新.
* **method** 只是一个Vue实例上的一个函数。当你显式调用的时候它才会计算。
###### 来源

* https://stackoverflow.com/questions/42936588/how-to-deploy-vue-app

[[↑] 返回顶部](#vuejs)
### 在Vue.js 2.0中兄弟组件间通信的正确方式是什么?

在Vue.js 2.0，我们可以使用eventHub机制。

思考下面代码:
```js
const eventHub = new Vue() // 单独的event hub

// 使用全局混入分配给组件
Vue.mixin({
    data: function () {
        return {
            eventHub: eventHub
        }
    }
})
// 你的组件可以用emit触发事件
this.eventHub.$emit('update', data)
// 监听你的你要做的
this.eventHub.$on('update', data => {
// 你要做的事情
})
```
你甚至可以在Vue根实例上使用`全局`的Event Hub让它变得更简洁:
```js
// 组件 1
this.$root.$emit('eventing', data);
// 组件 2
mounted() {
    this.$root.$on('eventing', data => {
        console.log(data);
    });
}
```

###### 来源

* https://stackoverflow.com/questions/42632711/how-to-call-function-on-child-component-on-parent-events

[[↑] 返回顶部](#vuejs)
### 如何在Vue.js切换class?

在Vue.js 2中你可以使用一个取决于数据属性isActive的布尔值来切换active class。

```html
<th 
  class="initial" 
  v-on:click="myFilter"
  v-bind:class="{ active: isActive }"
>
  <span class="wkday">M</span>
</th>
```

```js
methods: {
     myFilter: function(){          
        this.isActive = !this.isActive;
        // 过滤用户的代码
    }
}
```

###### 来源

* https://stackoverflow.com/questions/33731939/vue-js-toggle-class-on-click

[[↑] 返回顶部](#vuejs)
