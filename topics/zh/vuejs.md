## Vue.js

[如何创建 Vue 实例？](#如何创建-vue-实例)

[Vue.js 是什么？](#vuejs-是什么)

[Vue.js 中怎么使用本地存储？](#vuejs-中怎么使用本地存储)

[Vue.js 中如何创建双向绑定？](#vuejs-中如何创建双向绑定)

[Vue.js 的过滤器指什么？](#vuejs-的过滤器指什么)

[组件的 props 是什么？](#组件的-props-是什么)

[如何部署 Vue.js 应用？](#如何部署-vuejs-应用)

[Vue.js 的组件是什么？](#vuejs-的组件是什么)

[Vue.js 的指令是什么，列出一些你使用过的？](#vuejs-的指令是什么列出一些你使用过的)

[Vue.js 的过滤器是什么？](#vuejs-的过滤器是什么)

[列举一些 Vue.js 的特性](#列举一些-vuejs-的特性)

[Vue.js 中如何跳转到另一个页面？](#vuejs-中如何跳转到另一个页面)

[Vue.js 中我可以给计算属性传递参数吗？](#vuejs-中我可以给计算属性传递参数吗)

[解释一下 Vue.js 应用组织的基本逻辑](#解释一下-vuejs-应用组织的基本逻辑)

[Vue.js 的优/缺点是什么？](#vuejs-的优缺点是什么)

[解释下单向绑定和双向绑定的区别？](#解释下单向绑定和双向绑定的区别)

[Vue.js 中如何获取 URL 的查询参数？](#vuejs-中如何获取-url-的查询参数)

[列出 Vue.js 中的指令类型](#列出-vuejs-中的指令类型)

[如何在 Vue.js 中使用循环？](#如何在-vuejs-中使用循环)

[v-bind 和 v-model 的区别是什么？举例说明。](#v-bind-和-v-model-的区别是什么-举例说明)

[如何在父组件中调用子组件的函数？](#如何在父组件中调用子组件的函数)

[列举一些 Vue.js 的优点](#列举一些-vuejs-的优点)

[怎么给 Vue.js 过滤器传递参数？](#怎么给-vuejs-过滤器传递参数)

[如何避免 Vue.js 中的布局跳闪？](#如何避免-vuejs-中的布局跳闪)

[Gulp 和 Vue.js 如何配合使用？](#gulp-和-vuejs-如何配合使用)

[如何强制 Vue.js 重新加载/重新渲染？](#如何强制-vuejs-重新加载重新渲染)

[你知道 Vue.js 有些什么缺陷？](#你知道-vuejs-有些什么缺陷)

[Vue.js 中如何绑定 style？](#vuejs-中如何绑定-style)

[如何监听组件 props 的变化？](#如何监听组件-props-的变化)

[Vue.js 中有些什么和 Angular Service 相同的地方？](#vuejs-中有些什么和-angular-service-相同的地方)

[Vuex 是什么？](#vuex-是什么)

[Vue.js 如何在用户输入时将新值保存到本地存储中？](#vuejs-如何在用户输入时将新值保存到本地存储中)

[Vue.js 中如何实现一个简单的路由（不使用额外的库）？](#vuejs-中如何实现一个简单的路由不使用额外的库)

[列举一些 Vue.js 组件的通信方法](#列举一些-vuejs-组件的通信方法)

[Vue.js 中如何监听数组长度？](#vuejs-中如何监听数组长度)

[Vue.js 中为什么需要 mixins？](#vuejs-中为什么需要-mixins)

[创建可以从整个 Vue.js 应用访问的常量的最佳方法是什么？](#创建可以从整个-vuejs-应用访问的常量的最佳方法是什么)

[Vue.js 中方法和计算属性的主要区别是什么？](#vuejs-中方法和计算属性的主要区别是什么)

[Vue.js 2.0 中兄弟组件之间如何进行通信？](#vuejs-20-中兄弟组件之间如何进行通信)

[Vue.js 中如何切换 class？](#vuejs-中如何切换-class)

### 如何创建 Vue 实例？

每个 Vue 应用都是通过用 Vue 函数创建一个新的 Vue 实例开始的：

```js
var vm = new Vue({
  // 选项
});
```

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### Vue.js 是什么？

**Vue.js** 是一套用于构建用户界面的渐进式框架。它学起来很容易。要使用 Vue.js，你只需要给网站添加一点动态功能。你不用安装任何东西，只需要在你的项目中添加 Vue.js 库就行了。

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### Vue.js 中怎么使用本地存储？

你可以这么做：

```js
localStorage.setItem('YourItem', response.data);
localStorage.getItem('YourItem');
localStorage.removeItem('YourItem');
```

###### 来源

- https://stackoverflow.com/questions/41425889/vue-js-how-to-use-localstorage-with-vue-js

[[↑] 回到顶部](#vuejs)

### Vue.js 中如何创建双向绑定？

在 Vue.js 中你可以使用 `v-model` 指令创建双向绑定。双向绑定中，数据或模型与 DOM 绑定，DOM 绑定回模型。

通过下面的示例，你可以了解双向绑定是如何实现的。

```html
<div id="app">{{message}} <input v-model="message" /></div>
<script type="text/javascript">
  var message = 'Vue.js is rad';
  new Vue({ el: '#app', data: { message } });
</script>
```

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### Vue.js 的过滤器指什么？

Vue.js 中的过滤器，是用于对即将在浏览器上渲染的输出值进行格式化转换。

过滤器本质上是一个函数，接收一个参数值并经过相应处理，返回处理过后的值。在标记语言中，它由管道符号（|）表示，后面可以跟一个或多个参数：

```html
<element directive="expression | filterId \[args...\]"></element>
```

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### 组件的 props 是什么？

每个组件实例都有自己独立的作用域。这意味着你不能（也不应该）直接引用子组件模板中的父级数据。可以通过使用 **props** 将数据传递给子组件。props 是你可以在组件上注册的自定义属性。当一个值传递给某个 props 属性时，它就变成了那个组件实例上的一个属性。

```js
Vue.component('blog-post', {
  // JavaScript 中是 camelCase 命名法
  props: ['postTitle'],
  template: '<h3>{{ postTitle }}</h3>',
});
```

###### 来源

- https://vuejs.org/v2/guide/components-props.html#ad

[[↑] 回到顶部](#vuejs)

### 如何部署 Vue.js 应用？

如果你已经像这样创建了项目：

```sh
vue init webpack myproject
```

现在你可以在应用所在的目录下执行以下命令：

```sh
npm run build
```

然后复制 **index.html** 和 **/dist/ 文件夹** 到你网站服务器的根目录。以上。

###### 来源

- https://stackoverflow.com/questions/42936588/how-to-deploy-vue-app

[[↑] 回到顶部](#vuejs)

### Vue.js 的组件是什么？

*组件*是 Vue.js 最强大的特性之一。在 Vue.js 中，组件是自定义元素，扩展了基本的 HTML 元素，进而能对代码进行封装复用。

下面是在一个组件中注册另一个 Vue 组件的方法：

```js
export default {
  el: '#your-element',
  components: {
    'your-component'
  }
}
```

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### Vue.js 的指令是什么，列出一些你使用过的？

Vue.js 中的指令概念比 Angular 中的简单多了。Vue.js 指令使用新的属性和标签来扩展 HTML。Vue.js 有一组内置指令，给你的应用提供了扩展性功能。你还可以在 Vue.js 中编写自定义指令。

下面是一些 Vue.js 中常用的指令：

- v-show
- v-if
- v-model
- v-else
- v-on

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### Vue.js 的过滤器是什么？

Vue.js 允许你自定义过滤器，可被用于一些常见的文本格式化。过滤器可以用在两个地方：双花括号插值和 v-bind 表达式 (后者从 2.1.0+ 开始支持)。过滤器应该被添加在 JavaScript 表达式的尾部，由“管道”符号表示：

```html
<!-- 在双花括号中 -->
{{ message | capitalize }}

<!-- 在 `v-bind` 中 -->
<div v-bind:id="rawId | formatId"></div>
```

###### 来源

- https://vuejs.org/v2/guide/filters.html

[[↑] 回到顶部](#vuejs)

### 列举一些 Vue.js 的特性

Vue.js 有以下特性：

- 模板语法
- 响应式
- 组件化
- 过渡动画
- 路由

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### Vue.js 中如何跳转到另一个页面？

如果你使用 `vue-router`，你可以使用 `router.go(path)` 导航到其它特定路由，可以在组件内使用 `this.$ router` 访问路由属性。`router.go()` 在 Vue.js 2.0 版本中发生了变化。你可以使用 `router.push({name："yourroutename"})` 或只需 `router.push("yourroutename")` 便可以跳转。

[[↑] 回到顶部](#vuejs)

### Vue.js 中我可以给计算属性传递参数吗？

你可以使用 _方法_ 或 _计算属性_。

方法形式：

```js
<span>{{ fullName('Hi') }}</span>

methods: {
  fullName(salut) {
    return `${salut} ${this.firstName} ${this.lastName}`
  }
}
```

带参数计算属性形式：

```js
computed: {
  fullName() {
    return salut => `${salut} ${this.firstName} ${this.lastName}`
  }
}
```

[[↑] 回到顶部](#vuejs)

### 解释一下 Vue.js 应用组织的基本逻辑

一个 **Vue.js 应用** 由 new Vue 创建的根 Vue 实例组成，你可以编写复用组件进行嵌套组织，构成树状形式。例如，TODO 应用的组件树可能如下所示：

```sh
Root Instance
└─ TodoList
   ├─ TodoItem
   │  ├─ DeleteTodoButton
   │  └─ EditTodoButton
   └─ TodoListFooter
      ├─ ClearTodosButton
      └─ TodoListStatistics
```

所有 Vue 组件同样都是 Vue 实例。

###### 来源

- https://vuejs.org/v2/guide/instance.html

[[↑] 回到顶部](#vuejs)

### Vue.js 的优/缺点是什么？

**Vue.js 优点**

- 方便应用和界面开发
- 和 AngularJs 一样支持双向通信
- 支持状态控制
- 自然的框架思想流程

**Vue.js 缺点**

- 规模有限
- 只有一个创建者
- 开发者社区不大

[[↑] 回到顶部](#vuejs)

### 解释下单向绑定和双向绑定的区别？

单向数据流中，应用的视图（UI）部分不会在数据模型更改时自动更新，我们需要编写一些自定义代码，以便每次数据模型更改时更新它。在 Vue.js 中，我们使用**v-bind** 进行单向数据流绑定。

双向绑定中，应用的视图（UI）部分会在数据模型更改时自动更新。Vue.js 中，我们使用**v-model**指令进行双向数据绑定。

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### Vue.js 中如何获取 URL 的查询参数？

您可以在组件中访问 `$route` 对象，它提供了我们需要的  参数。

```js
// 组件内
console.log(this.$route.query.test);
```

###### 来源

- https://stackoverflow.com/questions/35914069/vue-js-query-parameters

[[↑] 回到顶部](#vuejs)

### 列出 Vue.js 中的指令类型

Vue.js 中有以下几种指令：

- 一般指令
- 文字指令
- 空指令
- 自定义指令

###### 来源

- https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] 回到顶部](#vuejs)

### 如何在 Vue.js 中使用循环?？

你可以这样构建模板：

```html
<b-menu v-for="menu in menu_items" v-bind:key="menu.label">
  <label>{{ menu.label }}</label>
  <b-menu-list v-for="item in menu.items" v-bind:key="item">
    <b-menu-item> {{ item.message }}</b-menu-item>
  </b-menu-list>
</b-menu>
```

###### 来源

- https://stackoverflow.com/questions/42260233/vue-js-difference-between-v-model-and-v-bind/44678583

[[↑] 回到顶部](#vuejs)

### v-bind 和 v-model 的区别是什么？举例说明。

`v-model` 用于**表单输入的双向绑定**。它结合了 `v-bind` 和 `v-on:input`，`v-bind` 负责传入 js 值给模板，`v-on:input` 负责更新 js 值。

代码如下：

```html
<input v-model="something" />
```

它是下面写法的语法糖：

```html
<input v-bind:value="something" v-on:input="something = $event.target.value" />
```

`v-model` 适用于所有原生 HTML input 类型（text, textarea, number, radio, checkbox, select）。 如果你想把日期数据存储为 ISO 字符串（`yyyy-mm-dd`）形式，可以把 `v-model` 与 `input type=date` 结合  使用。

###### 来源

- https://stackoverflow.com/questions/42260233/vue-js-difference-between-v-model-and-v-bind/44678583

[[↑] 回到顶部](#vuejs)

### 如何在父组件中调用子组件的函数？

给子组件设置 ref 属性，并通过 `$refs` 直接调用子组件上的方法。

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
  data: function() {
    return {
      value: 0,
    };
  },
  methods: {
    setValue: function(value) {
      this.value = value;
    },
  },
};

new Vue({
  el: '#app',
  components: {
    'child-component': ChildComponent,
  },
  methods: {
    click: function() {
      this.$refs.childComponent.setValue(2.0);
    },
  },
});
```

###### 来源

- https://stackoverflow.com/questions/42632711/how-to-call-function-on-child-component-on-parent-events

[[↑] 回到顶部](#vuejs)

### 列举一些 Vue.js 的优点

- 扩展 HTML。这说明 Vue.js 与 Angular 有许多相似的特性，我们可以通过划分不同组件来 优化 HTML 代码块。
- 详细的文档。Vue.js 有非常详细的文档，能有效地加快开发人员的学习进度，为应用开发节省了大量时间，并且只需要了解 HTML 和 JavaScript 的基本知识。
- 适应性。从其他框架切换到 Vue.js 不需要很长的适应时间，因为它的设计和架构与 Angular 和 React 较相似。
- 很棒的整合。Vue.js 可用于构建单页面应用或者更复杂的 Web 应用。最为重要的是，它轻量的交互部分可以轻松集成到现有基础架构中，而不会对整个系统产生副作用。
- 规模大。Vue.js 可以帮助开发者编写许多的可复用模板，简单的结构能为我们省下很多时间。
-  轻量。Vue.js 只有 20KB 左右大小，同时兼备速度和灵活性，与其它框架相比，性能更加。

###### 来源

- https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] 回到顶部](#vuejs)

### 怎么给 Vue.js 过滤器传递参数？

如下：

```js
filters:{
   currency: function(value, arg1){
     return arg1+value;
}
```

用法：

```html
<script src="https://cdnjs.cloudflare.com/ajax/libs/vue/2.5.1/vue.js"></script>
<div id="vue-instance">{{123 | currency('$') }}</div>
```

###### 来源

- https://vuejs.org/v2/guide/filters.html

[[↑] 回到顶部](#vuejs)

### 如何避免 Vue.js 中的布局跳闪？

要是你受不了首次渲染的时间，唯一的办法就是搞**服务器端渲染**。你的应用加载时便已经有了初始 html 结构。

[[↑] 回到顶部](#vuejs)

### Gulp 和 Vue.js 如何配合使用？

你可以使用 `Vueify`。它是 `browserify` 转换工具。

```js
gulp.task('browserify', function() {
  return gulp
    .src('src/js/main.js')
    .pipe(plumber())
    .pipe(
      browserify({
        debug: !env.p,
        transform: ['vueify'],
      })
    )
    .pipe(gulpif(env.p, uglify()))
    .pipe(gulp.dest('build/js'));
});
```

[[↑] 回到顶部](#vuejs)

### 如何强制 Vue.js 重新加载/重新渲染？

如下：

```js
vm.$forceUpdate();
```

###### 来源

- https://stackoverflow.com/questions/32106155/can-you-force-vue-js-to-reload-re-render

[[↑] 回到顶部](#vuejs)

### 你知道 Vue.js 有些什么缺陷？

- 缺乏资源。与 React 和 Angular 相比，Vue.js 的市场份额仍然很小，这意味着关于这个框架的资料分享仍处于起步阶段。
- 过于灵活的风险。有时候，把 Vue.js 整合进大型项目时可能会遇到问题，出现问题又找不到现成解决方案就完蛋，不过到时很快就会有相应解决方案。
- 中国背景。Vue.js 有一些中国背景，很多内容和说明都是中文的。这可能会导致框架维护发展阶段产生奇怪的问题，不过没关系，会有越来越多的资料翻译成英语的。

###### 来源

- https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] 回到顶部](#vuejs)

### Vue.js 中如何绑定 style？

如下：

```html
<div id="table">
  <div v-for="table in tables">
    <div class="table-div" v-bind:style="{top: table.top + 'px', left: table.left + 'px'}">
      {{table.name}}
    </div>
  </div>
</div>
```

###### 来源

- https://stackoverflow.com/questions/45604244/binding-styles-in-vue-js

[[↑] 回到顶部](#vuejs)

### 如何监听组件 props 的变化？

 当 props 改变时，你可以通过 `watch` props 来执行一些代码：

```js
new Vue({
  el: '#app',
  data: {
    text: 'Hello',
  },
  components: {
    child: {
      template: `<p>{{ myprop }}</p>`,
      props: ['myprop'],
      watch: {
        myprop: function(newVal, oldVal) {
          // 监听 myprop
          console.log('Prop changed: ', newVal, ' | was: ', oldVal);
        },
      },
    },
  },
});
```

在 HTML 中：

```html
<script src="https://unpkg.com/vue/dist/vue.js"></script>

<div id="app">
  <child :myprop="text"></child> <button @click="text = 'Another text'">Change text</button>
</div>
```

###### 来源

- https://stackoverflow.com/questions/44584292/vuejs-2-0-how-to-listen-for-props-changes

[[↑] 回到顶部](#vuejs)

### Vue.js 中有些什么和 Angular Service 相同的地方？

4 个地方：

- 无状态 service：那么你应该使用 mixins
- 有状态 service：使用 Vuex
- 从 vue 代码导出和导入 service
- 任意 javascript 全局对象

###### 来源

- https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] 回到顶部](#vuejs)

### Vuex 是什么？

Vuex 是 Vue.js 应用的**状态管理库**。它承担应用中所有组件的集中存储作用，它的规则保证了状态只能以可预测的方式进行变更。Vuex 背后的基础理念，受到 Flux，Redux 和 Elm 架构的启发。

Vuex 解决了两个问题：

- 多个视图可能依赖于同一状态。对于多层嵌套的组件，通过传递 props 会很麻烦，兄弟组件  则无法直接共享。
- 不同视图的操作可能会改变同一状态。我们会尝试自己寻找解决方案，例如直接操作父/子实例引用或尝试通过事件修改、同步状态的多个副本。这两种模式都不是很好，会导致代码难以维护。

###### 来源

- https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] 回到顶部](#vuejs)

### Vue.js 如何在用户输入时将新值保存到本地存储中？

使用 `watch` 方法检测存储数据的变化，如下所示：

```js
watch: {
  input: function () {
    if (isLocalStorage() /* 检测是否支持 localstorage 的函数*/) {
      localStorage.setItem('storedData', this.input)
    }
  }
}
```

###### 来源

- https://stackoverflow.com/questions/41425889/vue-js-how-to-use-localstorage-with-vue-js

[[↑] 回到顶部](#vuejs)

### Vue.js 中如何实现一个简单的路由（不使用额外的库）？

如果你只需要简单的路由功能，不涉及其它功能，可以通过动态渲染页面组件来实现，如下所示：

```js
const NotFound = { template: '<p>Page not found</p>' };
const Home = { template: '<p>home page</p>' };
const About = { template: '<p>about page</p>' };

const routes = {
  '/': Home,
  '/about': About,
};

new Vue({
  el: '#app',
  data: {
    currentRoute: window.location.pathname,
  },
  computed: {
    ViewComponent() {
      return routes[this.currentRoute] || NotFound;
    },
  },
  render(h) {
    return h(this.ViewComponent);
  },
});
```

对于大多数单页应用，建议使用官方支持的 vue-router 库。

###### 来源

- https://vuejs.org/v2/guide/routing.html

[[↑] 回到顶部](#vuejs)

### 列举一些 Vue.js 组件的通信方法

- **Props**（`props`）- Vue 中最简单的通信方法，用于父子组件直接通信。主要用于传递与逻辑有关的数据或层级有限的数据集。
- **Refs 和方法**（`ref`）- 当无法使用 prop 来让子组件处理父组件传递的事件时，可以在子组件上设置 ref 并调用它的方法。
- **事件**（`$emit`和`$on`）- 用于父子组件直接通信的简单方法。而且应该用于逻辑交互。
- **事件总线**（`this.$root.$emit`，`this.$root.$on`）- 当从祖先组件传递 props 到深层嵌套的子组件时比较有用，不过父子组件就不需要这样做了。
- **集中存储**（_Vuex_）- Vuex 是 Vue 的状态管理库。它不仅支持事件，还为应用提供了  完整的功能。

###### 来源

- https://stackoverflow.com/questions/38616167/communication-between-sibling-components-in-vuejs-2-0

[[↑] 回到顶部](#vuejs)

### Vue.js 中如何监听数组长度？

使用侦听器监听返回数组长度的计算属性：

```js
var vm = new Vue({
  el: 'body',
  data: {
    items: [],
  },
  computed: {
    item_length: function() {
      return this.battle_logs.length;
    },
  },
  watch: {
    items: {
      handler: function() {
        console.log('caught!');
      },
      deep: true,
    },
  },
});
```

或者

```js
vm.$watch('item_length', function(newVal, oldVal) {
  console.log('caught!');
});
```

###### 来源

- https://stackoverflow.com/questions/37041720/vue-js-watch-array-length

[[↑] 回到顶部](#vuejs)

### Vue.js 中为什么需要 mixins？

Mixins 是为 Vue 组件 _分发复用函数_ 的一种灵活方法。mixin 对象可以包含任何组件选项。当组件使用 mixin 时，mixin 中的所有选项将“混入”到组件自己的选项中。

代码如下：

```js
// 定义 mixin 对象
var myMixin = {
  methods: {
    getProducts() {
      myApi.get('products？id=' + prodId).then(response => (this.product = response.data));
    },
  },
};

// 定义使用 mixin 的组件
var Component = Vue.extend({
  mixins: [myMixin],
});

// 初始化时使用 mixin
new Vue({
  mixins: [myMixin],
  created: function() {
    console.log('other code');
  },
});
```

###### 来源

- https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] 回到顶部](#vuejs)

### 创建可以从整个 Vue.js 应用访问的常量的最佳方法是什么？

你始终可以在 Vue 应用的作用域外定义变量，并且可以在整个应用中使用它。

```js
//const.js
export default {
  c1: 'Constant 1',
  c2: 'Constant 2',
};
```

然后：

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

- https://stackoverflow.com/questions/46882944/what-is-the-best-way-to-create-a-constant-that-can-be-accessible-from-entire-ap

[[↑] 回到顶部](#vuejs)

### Vue.js 中方法和计算属性的主要区别是什么？

Vue.js 中，计算属性和方法在是完全不一样的，并且在大多数情况下不可互换。

- 计算值更合适的名称是**计算属性**。你可以将计算值视为派生值，只要用于计算的基础值更新，它就会 _自动_ 更新。
- **方法** 只是绑定到 Vue 实例的函数。只会在你 _显式调用_ 它时执行。

###### 来源

- https://stackoverflow.com/questions/42936588/how-to-deploy-vue-app

[[↑] 回到顶部](#vuejs)

### Vue.js 2.0 中兄弟组件之间如何进行通信？

Vue.js 2.0 中，我们可以使用 eventHub 机制。

如下：

```js
const eventHub = new Vue(); // 独立的事件注册中心

// 使用全局 mixin 分发给组件
Vue.mixin({
  data: function() {
    return {
      eventHub: eventHub,
    };
  },
});
// 你的组件可以触发事件
this.eventHub.$emit('update', data);
// 可以监听事件
this.eventHub.$on('update', data => {
  // 搞事情
});
```

你甚至可以将 Vue 根实例用作 `全局` 事件中心：

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

- https://stackoverflow.com/questions/42632711/how-to-call-function-on-child-component-on-parent-events

[[↑] 回到顶部](#vuejs)

### Vue.js 中如何切换 class？

你可以让 class 的激活状态依赖于某一布尔值：

```html
<th class="initial" v-on:click="myFilter" v-bind:class="{ active: isActive }">
  <span class="wkday">M</span>
</th>
```

```js
methods: {
     myFilter: function(){
        this.isActive = !this.isActive;
        // 一些过滤用户的代码
    }
}
```

###### 来源

- https://stackoverflow.com/questions/33731939/vue-js-toggle-class-on-click

[[↑] 回到顶部](#vuejs)
