## Vue.js

[How to create an instance of Vue.js? (Junior)](#how-to-create-an-instance-of-vuejs-junior)

[What is Vue.js? (Junior)](#what-is-vuejs-junior)

[What is Vue.js? (Junior)](#what-is-vuejs-junior)

[How to use local storage with Vue.js? (Mid)](#how-to-use-local-storage-with-vuejs-mid)

[How to create Two-Way Bindings in Vue.js? (Mid)](#how-to-create-two-way-bindings-in-vuejs-mid)

[What are filters in Vue.js? (Mid)](#what-are-filters-in-vuejs-mid)

[What are components props? (Mid)](#what-are-components-props-mid)

[How to deploy Vue.js app? (Mid)](#how-to-deploy-vuejs-app-mid)

[What are Components in Vue.js? (Mid)](#what-are-components-in-vuejs-mid)

[What are Directives in Vue.js, List some of them you used? (Mid)](#what-are-directives-in-vuejs-list-some-of-them-you-used-mid)

[What is filters in Vue.js? (Mid)](#what-is-filters-in-vuejs-mid)

[List some features of Vue.js (Mid)](#list-some-features-of-vuejs-mid)

[How can you redirect to another page in Vue.js? (Mid)](#how-can-you-redirect-to-another-page-in-vuejs-mid)

[Can I pass parameters in computer properties in Vue.js? (Mid)](#can-i-pass-parameters-in-computer-properties-in-vuejs-mid)

[Explain the basic logical Vue.js app organisation (Mid)](#explain-the-basic-logical-vuejs-app-organisation-mid)

[What are the Advantages/Disadvantages of Vuejs? (Mid)](#what-are-the-advantagesdisadvantages-of-vuejs-mid)

[Explain the differences between one-way data flow and two-way data binding? (Mid)](#explain-the-differences-between-one-way-data-flow-and-two-way-data-binding-mid)

[How can I fetch query parameters in Vue.js? (Mid)](#how-can-i-fetch-query-parameters-in-vuejs-mid)

[List type of Directive are available in Vue.js. (Senior)](#list-type-of-directive-are-available-in-vuejs-senior)

[How to loop in Vue.js? (Senior)](#how-to-loop-in-vuejs-senior)

[What is the difference v-bind and v-model? Provide some code example. (Senior)](#what-is-the-difference-v-bind-and-v-model-provide-some-code-example-senior)

[How to call function on child component on parent events? (Senior)](#how-to-call-function-on-child-component-on-parent-events-senior)

[List some benefits of Vue.js (Senior)](#list-some-benefits-of-vuejs-senior)

[How to pass an argument to Vue.js filters? (Senior)](#how-to-pass-an-argument-to-vuejs-filters-senior)

[How can you prevent layout jumps in Vue.js? (Senior)](#how-can-you-prevent-layout-jumps-in-vuejs-senior)

[How to use Gulp with Vue.js? (Expert)](#how-to-use-gulp-with-vuejs-expert)

[Can you force Vue.js to reload/rerender? (Expert)](#can-you-force-vuejs-to-reloadrerender-expert)

[Are there any drawback of Vue.js you know? (Expert)](#are-there-any-drawback-of-vuejs-you-know-expert)

[How can you bind styles in Vue.js? (Expert)](#how-can-you-bind-styles-in-vuejs-expert)

[Could you listen for components props changes? (Expert)](#could-you-listen-for-components-props-changes-expert)

[What's the equivalent of Angular Service in Vue.js? (Expert)](#whats-the-equivalent-of-angular-service-in-vuejs-expert)

[What is Vuex? (Expert)](#what-is-vuex-expert)

[How to save new value to data variables in Vue.js whenever the user types? (Expert)](#how-to-save-new-value-to-data-variables-in-vuejs-whenever-the-user-types-expert)

[How to implement simple routing in Vue.js (without external library)? (Expert)](#how-to-implement-simple-routing-in-vuejs-without-external-library-expert)

[List some types of components communication channels in Vue.js app (Expert)](#list-some-types-of-components-communication-channels-in-vuejs-app-expert)

[How can I watch an array length using Vue.js? (Expert)](#how-can-i-watch-an-array-length-using-vuejs-expert)

[Why we need Vue.js mixins? (Expert)](#why-we-need-vuejs-mixins-expert)

[What is the best way to create a constant, that can be accessible from entire application in VueJs ? (Expert)](#what-is-the-best-way-to-create-a-constant-that-can-be-accessible-from-entire-application-in-vuejs--expert)

[What is the main difference between a method and a computed value in Vue.js? (Expert)](#what-is-the-main-difference-between-a-method-and-a-computed-value-in-vuejs-expert)

[What is a proper way to communicate between sibling components in vuejs 2.0? (Expert)](#what-is-a-proper-way-to-communicate-between-sibling-components-in-vuejs-20-expert)

[How do you toggle a class in Vue.js? (Expert)](#how-do-you-toggle-a-class-in-vuejs-expert)



### How to create an instance of Vue.js? (Junior)

Every Vue application starts by creating a new Vue instance with the Vue function:

```js
var vm = new Vue({
  // options
})
```

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### What is Vue.js? (Junior)

The **Vue.js** is a progressive JavaScript framework and used to building the interactive user interfaces and also it’s focused on the view layer only (front end). The  **Vue.js**  was developed by “**Evan You**”, an Ex Google software engineer. The latest version is Vue.js 2. The Vue.js 2 is very similar to Angular because Evan You was inspired by Angular.

###### Source

* 

[[↑] Back to top](#Vue.js)
### What is Vue.js? (Junior)

**Vue js** is progressive javascript script used to create dynamic user interfaces.Vue js is very easy to learn.In order to work with Vue js you just need to add few dynamic features to a website.You don’t need to install any thing to use Vue js just need add Vue js library in your project.

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### How to use local storage with Vue.js? (Mid)

You can just do following:

```js
localStorage.setItem('YourItem', response.data)
localStorage.getItem('YourItem')
localStorage.removeItem('YourItem')
```

###### Source

* https://stackoverflow.com/questions/41425889/vue-js-how-to-use-localstorage-with-vue-js

[[↑] Back to top](#Vue.js)
### How to create Two-Way Bindings in Vue.js? (Mid)

`v-model` directive is used to create Two-Way Bindings in Vue js.In Two-Way Bindings data or model is bind with DOM and Dom is binded back to model.

In below example you can see how Two-Way Bindings is implemented.

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

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### What are filters in Vue.js? (Mid)

In Vue js filters are used to transform the output that are going to rendered on browser.

A Vue.js filter is essentially a function that takes a value, processes it, and then returns the processed value. In the markup it is denoted by a single pipe (|) and can be followed by one or more arguments:

```html
<element directive="expression | filterId \[args...\]"></element>
```

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### What are components props? (Mid)

Every component instance has its own isolated scope. This means you cannot (and should not) directly reference parent data in a child component’s template. Data can be passed down to child components using **props**. Props are custom attributes you can register on a component. When a value is passed to a prop attribute, it becomes a property on that component instance.

```js
Vue.component('blog-post', {
  // camelCase in JavaScript
  props: ['postTitle'],
  template: '<h3>{{ postTitle }}</h3>'
})
```

###### Source

* https://vuejs.org/v2/guide/components-props.html#ad

[[↑] Back to top](#Vue.js)
### How to deploy Vue.js app? (Mid)

If you've created your project like this:
```sh
vue init webpack myproject
```
Now you can run
```sh
npm run build
```
Then copy index.html and /dist/ folder into your website root directory. Done.

###### Source

* https://stackoverflow.com/questions/42936588/how-to-deploy-vue-app

[[↑] Back to top](#Vue.js)
### What are Components in Vue.js? (Mid)

*Components* are one of most powerful features of Vue js.In Vue components are custom elements that help extend basic HTML elements to encapsulate reusable code.

Following is the way to register a Vue component inside another component:
```js
export default {
  el: '#your-element'
  components: {
      'your-component'
  }
}
```

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### What are Directives in Vue.js, List some of them you used? (Mid)

The concept of directive in Vue js is drastically simpler than that in Angular. Vue.js directives provides a way to extend HTML with new attributes and tags. Vue.js has a set of built-in directives which offers extended functionality to your applications.You can also write your custom directives in Vue.js .

Below are list of commonly used directives in Vue.js

*   v-show
*   v-if
*   v-model
*   v-else
*   v-on

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### What is filters in Vue.js? (Mid)

Vue.js allows you to define **filters** that can be used to apply common text formatting. Filters are usable in two places: mustache interpolations and v-bind expressions (the latter supported in 2.1.0+). Filters should be appended to the end of the JavaScript expression, denoted by the “pipe” symbol:

```html
<!-- in mustaches -->
{{ message | capitalize }}

<!-- in v-bind -->
<div v-bind:id="rawId | formatId"></div>
```

###### Source

* https://vuejs.org/v2/guide/filters.html

[[↑] Back to top](#Vue.js)
### List some features of Vue.js (Mid)

Vue js comes with following features

*   Templates
*   Reactivity
*   Components
*   Transitions
*   Routing

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### How can you redirect to another page in Vue.js? (Mid)

If you are using  `vue-router`, you should use  `router.go(path)`  to navigate to any particular route. The router can be accessed from within a component using  `this.$router`.  `router.go()`  changed in VueJS 2.0. You can use  `router.push({ name: "yourroutename"})`or just  `router.push("yourroutename")`  now to redirect. 


###### Source

* 

[[↑] Back to top](#Vue.js)
### Can I pass parameters in computer properties in Vue.js? (Mid)

You can use a _method_ or _computed function_.

The method way:

```js
<span>{{ fullName('Hi') }}</span>

methods: {
  fullName(salut) {
      return `${salut} ${this.firstName} ${this.lastName}`
  }
}
```
Computed property with a parameter way:

```js
computed: { 
	fullName() {
		return salut => `${salut} ${this.firstName} 		
		 ${this.lastName}`
    }
}
```

###### Source

* 

[[↑] Back to top](#Vue.js)
### Explain the basic logical Vue.js app organisation (Mid)

A **Vue.js application** consists of a root Vue instance created with new Vue, optionally organized into a tree of nested, reusable components. For example, a todo app’s component tree might look like this:

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
All Vue components are also Vue instances.

###### Source

* https://vuejs.org/v2/guide/instance.html

[[↑] Back to top](#Vue.js)
### What are the Advantages/Disadvantages of Vuejs? (Mid)

**Vue.js Advantages**
- Easy for applications and interfaces development
- Support Two-way communication as like AngularJs
- Ability to control the states
- Natural thought process

**Vue.js** **Disadvantages**
- Limited scope
- Single creator
- Small developer community

###### Source

* 

[[↑] Back to top](#Vue.js)
### Explain the differences between one-way data flow and two-way data binding? (Mid)

In one-way data flow the view(UI) part of application does not updates automatically when data Model is change  we need to write some custom code to make it updated every time a data model is changed. In Vue js **v-bind** is used for one-way data flow or binding.

In two-way data binding the view(UI) part of application automatically updates when data Model is changed.  In Vue.js **v-model** directive is used for two way data binding.

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### How can I fetch query parameters in Vue.js? (Mid)

You have access to a `$route` object from your components, that expose what we need.

```js    
//from your component
console.log(this.$route.query.test)
```

###### Source

* https://stackoverflow.com/questions/35914069/vue-js-query-parameters

[[↑] Back to top](#Vue.js)
### List type of Directive are available in Vue.js. (Senior)

In Vue.js following types of directives are available

*   General Directives
*   Literal Directives
*   Empty Directives
*   Custom Directives

###### Source

* https://www.onlineinterviewquestions.com/vue-js-interview-questions/#.Wx0soFOFNTY

[[↑] Back to top](#Vue.js)
### How to loop in Vue.js? (Senior)

You could build your template this way:

```html
<b-menu v-for="menu in menu_items" v-bind:key="menu.label">
    <label>{{ menu.label }}</label>
    <b-menu-list v-for="item in menu.items" v-bind:key="item">
        <b-menu-item> {{ item.message }}</b-menu-item>
    </b-menu-list>
</b-menu>
```

###### Source

* https://stackoverflow.com/questions/42260233/vue-js-difference-between-v-model-and-v-bind/44678583

[[↑] Back to top](#Vue.js)
### What is the difference v-bind and v-model? Provide some code example. (Senior)

`v-model`  is a  **two-way binding for form inputs**. It combines  `v-bind`, which  **_brings a js value_ **into the markup, and  `v-on:input`  to  **_update the js value_**.

Consider:
```html
<input v-model="something">
```
and it's just syntactic sugar for:
```html
<input
   v-bind:value="something"
   v-on:input="something = $event.target.value"
>
```

`v-model`  works with all the basic HTML input types (text, textarea, number, radio, checkbox, select). You can use  `v-model`  with  `input type=date`  if your model stores dates as ISO strings (`yyyy-mm-dd`).

###### Source

* https://stackoverflow.com/questions/42260233/vue-js-difference-between-v-model-and-v-bind/44678583

[[↑] Back to top](#Vue.js)
### How to call function on child component on parent events? (Senior)

Give the child component a ref and use `$refs` to call a method on the child component directly.

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

###### Source

* https://stackoverflow.com/questions/42632711/how-to-call-function-on-child-component-on-parent-events

[[↑] Back to top](#Vue.js)
### List some benefits of Vue.js (Senior)

* Empowered HTML. This means that Vue.js has many similar characteristics with Angular and this can help to optimize HTML blocks handling with a usage of different components.
* Detailed documentation. Vue.js has very circumstantial documentation which can fasten learning curve for developers and save a lot of time to develop an app using only the basic knowledge of HTML and JavaScript.
* Adaptability. It provides a rapid switching period from other frameworks to Vue.js because of the similarity with Angular and React in terms of design and architecture.
* Awesome integration. Vue.js can be used for both building single-page applications and more difficult web interfaces of apps. The main thing is that smaller interactive parts can be easily integrated into the existing infrastructure with no negative effect on the entire system.
* Large scaling. Vue.js can help to develop pretty large reusable templates that can be made with no extra time allocated for that according to its simple structure.
* Tiny size. Vue.js can weight around 20KB keeping its speed and flexibility that allows reaching much better performance in comparison to other frameworks.

###### Source

* https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] Back to top](#Vue.js)
### How to pass an argument to Vue.js filters? (Senior)

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

[[↑] Back to top](#Vue.js)
### How can you prevent layout jumps in Vue.js? (Senior)

You want to totally nullify the time of the first rendering, the only way to go is to do **server-side rendering**. So your app will be served with the initial html structure already there.

###### Source

* 

[[↑] Back to top](#Vue.js)
### How to use Gulp with Vue.js? (Expert)

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

###### Source

* 

[[↑] Back to top](#Vue.js)
### Can you force Vue.js to reload/rerender? (Expert)

Yes. Consider:
```js
vm.$forceUpdate();
```

###### Source

* https://stackoverflow.com/questions/32106155/can-you-force-vue-js-to-reload-re-render

[[↑] Back to top](#Vue.js)
### Are there any drawback of Vue.js you know? (Expert)

* Lack of resources. Vue.js still has a pretty small market share in comparison with React or Angular, which means that knowledge sharing in this framework is still in the beginning phase.
* Risk of over flexibility. Sometimes, Vue.js might have issues while integrating into huge projects and there is still no experience with possible solutions, but they will definitely come soon.
* Chinese background. As far as Vue.js has a bit of Chinese background, a lot of elements and descriptions are still available in Chinese. This leads to a partial complexity on some stages of development, nevertheless, more and more materials are being translated into English.

###### Source

* https://medium.com/@TechMagic/reactjs-vs-angular5-vs-vue-js-what-to-choose-in-2018-b91e028fa91d

[[↑] Back to top](#Vue.js)
### How can you bind styles in Vue.js? (Expert)

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

[[↑] Back to top](#Vue.js)
### Could you listen for components props changes? (Expert)

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

[[↑] Back to top](#Vue.js)
### What's the equivalent of Angular Service in Vue.js? (Expert)

There are 4 ways:

* Stateless service: then you should use mixins
* Statefull service: use Vuex
* Export service and import from a vue code
* any javascript global object

###### Source

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] Back to top](#Vue.js)
### What is Vuex? (Expert)


Vuex is a **state management pattern + library** for Vue.js applications. It serves as a centralized store for all the components in an application, with rules ensuring that the state can only be mutated in a predictable fashion. The basic idea behind Vuex, inspired by Flux, Redux and The Elm Architecture.

Vuex resolves two problems:
* Multiple views may depend on the same piece of state. Passing props can be tedious for deeply nested components, and simply doesn't work for sibling components. 
* Actions from different views may need to mutate the same piece of state. We often find ourselves resorting to solutions such as reaching for direct parent/child instance references or trying to mutate and synchronize multiple copies of the state via events. Both of these patterns are brittle and quickly lead to unmaintainable code.

###### Source

* https://stackoverflow.com/questions/41164672/whats-the-equivalent-of-angular-service-in-vuejs

[[↑] Back to top](#Vue.js)
### How to save new value to data variables in Vue.js whenever the user types? (Expert)

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

[[↑] Back to top](#Vue.js)
### How to implement simple routing in Vue.js (without external library)? (Expert)

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

[[↑] Back to top](#Vue.js)
### List some types of components communication channels in Vue.js app (Expert)

* **Props** (`props`) - The simplest communication channel in Vue for direct Parent-Child communication. It should mostly be used to pass data relating to presentation logic or a restricted set of data down the hierarchy.
* **Refs and methods** (`ref`) - When it doesn't make sense to use a prop to let a child handle an event from a parent, setting up a ref on the child component and calling its methods is just fine.
* **Events** (`$emit` and `$on`) - The simplest communication channel for direct Child-Parent communication. Again, should be used for presentation logic.
* **Event bus** (`this.$root.$emit`, `this.$root.$on`) - This can become useful when passing props all over the place from far up down to deeply nested children components, with almost no other components needing these in between.
* **Centralized store** (_Vuex_) - Vuex is the way to go with Vue for state management. It offers a lot more than just events and it's ready for full scale application.


###### Source

* https://stackoverflow.com/questions/38616167/communication-between-sibling-components-in-vuejs-2-0

[[↑] Back to top](#Vue.js)
### How can I watch an array length using Vue.js? (Expert)

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

[[↑] Back to top](#Vue.js)
### Why we need Vue.js mixins? (Expert)

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

[[↑] Back to top](#Vue.js)
### What is the best way to create a constant, that can be accessible from entire application in VueJs ? (Expert)

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

[[↑] Back to top](#Vue.js)
### What is the main difference between a method and a computed value in Vue.js? (Expert)

Computed values and methods are very different in Vue and are definitely not interchangeable in most cases.
* A more appropriate name for a computed value is a **computed property**. You can think of a computed value as a derived value that will be _automatically_ updated whenever one of the underlying values used to calculate it is updated.
* A **method** is just a function bound to the Vue instance. It will only be evaluated when you _explicitly call_ it. 

###### Source

* https://stackoverflow.com/questions/42936588/how-to-deploy-vue-app

[[↑] Back to top](#Vue.js)
### What is a proper way to communicate between sibling components in vuejs 2.0? (Expert)

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

[[↑] Back to top](#Vue.js)
### How do you toggle a class in Vue.js? (Expert)

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

[[↑] Back to top](#Vue.js)
