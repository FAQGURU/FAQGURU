## Vue.js

[如何创建一个vuejs实例?](#如何创建一个vuejs实例)

[Vue.js是什么?](#vuejs是什么)

[如何在Vue.js中使用local storage?](#如何在vuejs中使用local-storage)

[如何在Vue.js中创建双向绑定?](#如何在vuejs中创建双向绑定)

[Vue.js的过滤器是什么(一)?](#vuejs的过滤器是什么一)

[组件的props是什么?](#组件的props是什么)

[如何部署一个Vue.js app?](#如何部署一个vuejs-app)

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

[List some benefits of Vue.js](#list-some-benefits-of-vuejs)

[How to pass an argument to Vue.js filters?](#how-to-pass-an-argument-to-vuejs-filters)

[How can you prevent layout jumps in Vue.js?](#how-can-you-prevent-layout-jumps-in-vuejs)

[How to use Gulp with Vue.js?](#how-to-use-gulp-with-vuejs)

[Can you force Vue.js to reload/rerender?](#can-you-force-vuejs-to-reloadrerender)

[Are there any drawback of Vue.js you know?](#are-there-any-drawback-of-vuejs-you-know)

[How can you bind styles in Vue.js?](#how-can-you-bind-styles-in-vuejs)

[Could you listen for components props changes?](#could-you-listen-for-components-props-changes)

[What's the equivalent of Angular Service in Vue.js?](#whats-the-equivalent-of-angular-service-in-vuejs)

[What is Vuex?](#what-is-vuex)

[How to save new value to data variables in Vue.js whenever the user types?](#how-to-save-new-value-to-data-variables-in-vuejs-whenever-the-user-types)

[How to implement simple routing in Vue.js (without external library)?](#how-to-implement-simple-routing-in-vuejs-without-external-library)

[List some types of components communication channels in Vue.js app](#list-some-types-of-components-communication-channels-in-vuejs-app)

[How can I watch an array length using Vue.js?](#how-can-i-watch-an-array-length-using-vuejs)

[Why we need Vue.js mixins?](#why-we-need-vuejs-mixins)

[What is the best way to create a constant, that can be accessible from entire application in VueJs ?](#what-is-the-best-way-to-create-a-constant-that-can-be-accessible-from-entire-application-in-vuejs-)

[What is the main difference between a method and a computed value in Vue.js?](#what-is-the-main-difference-between-a-method-and-a-computed-value-in-vuejs)

[What is a proper way to communicate between sibling components in vuejs 2.0?](#what-is-a-proper-way-to-communicate-between-sibling-components-in-vuejs-20)

[How do you toggle a class in Vue.js?](#how-do-you-toggle-a-class-in-vuejs)



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
### 如何部署一个Vue.js app?

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
### List some benefits of Vue.js

* Empowered HTML. This means that Vue.js has many similar characteristics with Angular and this can help to optimize HTML blocks handling with a usage of different components.
* Detailed documentation. Vue.js has very circumstantial documentation which can fasten learning curve for developers and save a lot of time to develop an app using only the basic knowledge of HTML and JavaScript.
* Adaptability. It provides a rapid switching period from other frameworks to Vue.js because of the similarity with Angular and React in terms of design and architecture.
* Awesome integration. Vue.js can be used for both building single-page applications and more difficult web interfaces of apps. The main thing is that smaller interactive parts can be easily integrated into the existing infrastructure with no negative effect on the entire system.
* Large scaling. Vue.js can help to develop pretty large reusable templates that can be made with no extra time allocated for that according to its simple structure.
* Tiny size. Vue.js can weight around 20KB keeping its speed and flexibility that allows reaching much better performance in comparison to other frameworks.

###### Source

* https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] Back to top](#vuejs)
### How to pass an argument to Vue.js filters?

Consider:
```js
filters:{
   currency: function(value, arg1){
     return arg1+value;
}
```
And usage:
```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.5.1/vue.js"></script>
<div id="vue-instance">
  {{123 | currency('$') }}
</div>
```

###### Source

* https://vuejs.org/v2/guide/filters.html

[[↑] Back to top](#vuejs)
### How can you prevent layout jumps in Vue.js?

You want to totally nullify the time of the first rendering, the only way to go is to do **server-side rendering**. So your app will be served with the initial html structure already there.

[[↑] Back to top](#vuejs)
### How to use Gulp with Vue.js?

You can use `Vueify`. it's a `browserify` transform.

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

[[↑] Back to top](#vuejs)
### Can you force Vue.js to reload/rerender?

Yes. Consider:
```js
vm.$forceUpdate();
```

###### Source

* https://stackoverflow.com/questions/32106155/can-you-force-vue-js-to-reload-re-render

[[↑] Back to top](#vuejs)
### Are there any drawback of Vue.js you know?

* Lack of resources. Vue.js still has a pretty small market share in comparison with React or Angular, which means that knowledge sharing in this framework is still in the beginning phase.
* Risk of over flexibility. Sometimes, Vue.js might have issues while integrating into huge projects and there is still no experience with possible solutions, but they will definitely come soon.
* Chinese background. As far as Vue.js has a bit of Chinese background, a lot of elements and descriptions are still available in Chinese. This leads to a partial complexity on some stages of development, nevertheless, more and more materials are being translated into English.

###### Source

* https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] Back to top](#vuejs)
### How can you bind styles in Vue.js?

Consider:
```html
<div id="table">
    <div v-for="table in tables">
        <div class="table-div" v-bind:style="{top: table.top + 'px', left: table.left + 'px'}">{{table.name}}</div>
    </div>
</div>
```

###### Source

* https://stackoverflow.com/questions/45604244/binding-styles-in-vue-js

[[↑] Back to top](#vuejs)
### Could you listen for components props changes?

Yes. You can `watch` props to execute some code upon props changes:
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
And in HTML:
```html
<script src="https://unpkg.com/vue/dist/vue.js"></script>

<div id="app">
  <child :myprop="text"></child>
  <button @click="text = 'Another text'">Change text</button>
</div>
```

###### Source

* https://stackoverflow.com/questions/44584292/vuejs-2-0-how-to-listen-for-props-changes

[[↑] Back to top](#vuejs)
### What's the equivalent of Angular Service in Vue.js?

There are 4 ways:

* Stateless service: then you should use mixins
* Statefull service: use Vuex
* Export service and import from a vue code
* any javascript global object

###### Source

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] Back to top](#vuejs)
### What is Vuex?


Vuex is a **state management pattern + library** for Vue.js applications. It serves as a centralized store for all the components in an application, with rules ensuring that the state can only be mutated in a predictable fashion. The basic idea behind Vuex, inspired by Flux, Redux and The Elm Architecture.

Vuex resolves two problems:
* Multiple views may depend on the same piece of state. Passing props can be tedious for deeply nested components, and simply doesn't work for sibling components. 
* Actions from different views may need to mutate the same piece of state. We often find ourselves resorting to solutions such as reaching for direct parent/child instance references or trying to mutate and synchronize multiple copies of the state via events. Both of these patterns are brittle and quickly lead to unmaintainable code.

###### Source

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] Back to top](#vuejs)
### How to save new value to data variables in Vue.js whenever the user types?

Use `watch` method to detect changes on variable you are storing data on like this:

```js
watch: {
  input: function () {
    if (isLocalStorage() /* function to detect if localstorage is supported*/) {
      localStorage.setItem('storedData', this.input)
    }
  }
}
```

###### Source

* https://stackoverflow.com/questions/41425889/vue-js-how-to-use-localstorage-with-vue-js

[[↑] Back to top](#vuejs)
### How to implement simple routing in Vue.js (without external library)?

If you only need very simple routing and do not wish to involve a full-featured router library, you can do so by dynamically rendering a page-level component like this:

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
For most Single Page Applications, it’s recommended to use the officially-supported vue-router library.

###### Source

* https://vuejs.org/v2/guide/routing.html

[[↑] Back to top](#vuejs)
### List some types of components communication channels in Vue.js app

* **Props** (`props`) - The simplest communication channel in Vue for direct Parent-Child communication. It should mostly be used to pass data relating to presentation logic or a restricted set of data down the hierarchy.
* **Refs and methods** (`ref`) - When it doesn't make sense to use a prop to let a child handle an event from a parent, setting up a ref on the child component and calling its methods is just fine.
* **Events** (`$emit` and `$on`) - The simplest communication channel for direct Child-Parent communication. Again, should be used for presentation logic.
* **Event bus** (`this.$root.$emit`, `this.$root.$on`) - This can become useful when passing props all over the place from far up down to deeply nested children components, with almost no other components needing these in between.
* **Centralized store** (_Vuex_) - Vuex is the way to go with Vue for state management. It offers a lot more than just events and it's ready for full scale application.


###### Source

* https://stackoverflow.com/questions/38616167/communication-between-sibling-components-in-vuejs-2-0

[[↑] Back to top](#vuejs)
### How can I watch an array length using Vue.js?

Use the watch section in your vm creation:
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
Or watch a computed length attribute:
```js
vm.$watch('item_length', function(newVal, oldVal) {
    console.log('caught!');
});
```

###### Source

* https://stackoverflow.com/questions/37041720/vue-js-watch-array-length

[[↑] Back to top](#vuejs)
### Why we need Vue.js mixins?

Mixins are a flexible way to _distribute reusable functionalities_ for Vue components. A mixin object can contain any component options. When a component uses a mixin, all options in the mixin will be “mixed” into the component’s own options. 

Consider:
```js
// define a mixin object
var myMixin = {
  methods: {
     getProducts () {
         myApi.get('products?id=' + prodId).then(response =>  this.product = response.data)
      }
  }
}

// define a component that uses this mixin
var Component = Vue.extend({
  mixins: [myMixin]
})

// alternate way to have a mixin while initialising
new Vue({
  mixins: [myMixin],
  created: function () {
    console.log('other code')
  }
})
```

###### Source

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] Back to top](#vuejs)
### What is the best way to create a constant, that can be accessible from entire application in VueJs ?

You can always define a variable outside of the Vue app scope and use it throughout the application.

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

###### Source

* https://stackoverflow.com/questions/46882944/what-is-the-best-way-to-create-a-constant-that-can-be-accessible-from-entire-ap

[[↑] Back to top](#vuejs)
### What is the main difference between a method and a computed value in Vue.js?

Computed values and methods are very different in Vue and are definitely not interchangeable in most cases.
* A more appropriate name for a computed value is a **computed property**. You can think of a computed value as a derived value that will be _automatically_ updated whenever one of the underlying values used to calculate it is updated.
* A **method** is just a function bound to the Vue instance. It will only be evaluated when you _explicitly call_ it. 

###### Source

* https://stackoverflow.com/questions/42936588/how-to-deploy-vue-app

[[↑] Back to top](#vuejs)
### What is a proper way to communicate between sibling components in vuejs 2.0?

With Vue 2.0, we using the eventHub mechanism.

Consider:
```js
const eventHub = new Vue() // Single event hub

// Distribute to components using global mixin
Vue.mixin({
    data: function () {
        return {
            eventHub: eventHub
        }
    }
})
// your component you can emit events with
this.eventHub.$emit('update', data)
// And to listen you do
this.eventHub.$on('update', data => {
// do your thing
})
```
You can even make it shorter and use root Vue instance as `global` Event Hub:
```js
// Component 1
this.$root.$emit('eventing', data);
// Component 2
mounted() {
    this.$root.$on('eventing', data => {
        console.log(data);
    });
}
```

###### Source

* https://stackoverflow.com/questions/42632711/how-to-call-function-on-child-component-on-parent-events

[[↑] Back to top](#vuejs)
### How do you toggle a class in Vue.js?

For Vue.js 2 you could have the active class be dependent upon a boolean data value:

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
        // some code to filter users
    }
}
```

###### Source

* https://stackoverflow.com/questions/33731939/vue-js-toggle-class-on-click

[[↑] Back to top](#vuejs)
