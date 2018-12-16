## Redux

[What is Flux?](#what-is-flux)

[What is Redux DevTools?](#what-is-redux-devtools)

[What is Redux?](#what-is-redux)

[Do you need to keepIs all component states in Redux store?](#do-you-need-to-keepis-all-component-states-in-redux-store)

[How to add multiple middlewares to Redux?](#how-to-add-multiple-middlewares-to-redux)

[What are Redux selectors and Why to use them?](#what-are-redux-selectors-and-why-to-use-them)

[What are the features of Redux DevTools?](#what-are-the-features-of-redux-devtools)

[What are reducers in redux?](#what-are-reducers-in-redux)

[What is Redux Thunk?](#what-is-redux-thunk)

[What is the difference between React context and React redux?](#what-is-the-difference-between-react-context-and-react-redux)

[What is redux-saga?](#what-is-redux-saga)

[What are the core principles of Redux?](#what-are-the-core-principles-of-redux)

[How to set initial state in Redux?](#how-to-set-initial-state-in-redux)

[How to structure Redux top level directories?](#how-to-structure-redux-top-level-directories)

[What are the downsides of Redux over Flux?](#what-are-the-downsides-of-redux-over-flux)

[What are the differences between redux-saga and redux-thunk?](#what-are-the-differences-between-redux-saga-and-redux-thunk)

[What is the purpose of the constants in Redux?](#what-is-the-purpose-of-the-constants-in-redux)

[How to use connect from react redux?](#how-to-use-connect-from-react-redux)

[Are there any similarities between Redux and RxJS?](#are-there-any-similarities-between-redux-and-rxjs)

[What is Redux form?](#what-is-redux-form)

[What are the main features of Redux Form?](#what-are-the-main-features-of-redux-form)

[How to access redux store outside a react component?](#how-to-access-redux-store-outside-a-react-component)

[What is the proper way to access Redux store?](#what-is-the-proper-way-to-access-redux-store)

[What are the differences between call and put in redux-saga?](#what-are-the-differences-between-call-and-put-in-redux-saga)

[Whats the purpose of at (@) symbol in the redux connect decorator?](#whats-the-purpose-of-at--symbol-in-the-redux-connect-decorator)

[How to make Ajax request in Redux?](#how-to-make-ajax-request-in-redux)

[Why are Redux state functions called as reducers?](#why-are-redux-state-functions-called-as-reducers)

[How to reset state in redux?](#how-to-reset-state-in-redux)

[What is the mental model of redux-saga?](#what-is-the-mental-model-of-redux-saga)

[How Relay is different from Redux?](#how-relay-is-different-from-redux)



### What is Flux?

**Flux** is an application design paradigm used as a replacement for the more traditional mvc pattern. It is not a framework or a library but a new kind of architecture that complements React and the concept of Unidirectional Data Flow. Facebook used this pattern internally when working with React The workflow between dispatcher, stores and views components with distinct inputs and outputs as follows:

<div class="text-center"/>
<img src="https://github.com/sudheerj/reactjs-interview-questions/raw/master/images/flux.png" class="img-fluid"/>
</div>


###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is Redux DevTools?

**Redux DevTools** is a live-editing time travel environment for redux with hot reloading, action replay, and customizable UI. If you don’t want to bother with installing Redux DevTools and integrating it into your project, consider using Redux DevTools Extension for Chrome and Firefox.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is Redux?

**Redux** is a predictable state container for JavaScript apps based on the Flux design pattern. Redux can be used together with ReactJS, or with any other view library. It is tiny (about 2kB) and has no dependencies.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### Do you need to keepIs all component states in Redux store?

You need to keep your application state as small as possible. You don't have to push everything in there. Only do it makes a lot of sense to keep something there Or if it makes your life easier when using Dev Tools. But we shouldn't overload its importance too much.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How to add multiple middlewares to Redux?

You can use `applyMiddleware` where you can pass each piece of middleware as a new argument. So you just need to pass each piece of middleware you'd like. For example, you can add Redux Thunk and logger middlewares as an argument as below,
```js
import { createStore, applyMiddleware } from 'redux'
const createStoreWithMiddleware = applyMiddleware(ReduxThunk, logger)(createStore);

```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are Redux selectors and Why to use them?

Selectors are functions that take Redux state as an argument and return some data to pass to the component.
For example, to get user details from the state:
```js
const getUserData = state => state.user.data;
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are the features of Redux DevTools?

Below are the major features of Redux devTools
1. Lets you inspect every state and action payload
2. Lets you go back in time by “cancelling” actions
3. If you change the reducer code, each “staged” action will be re-evaluated
4. If the reducers throw, you will see during which action this happened, and what the error was
5. With `persistState()` store enhancer, you can persist debug sessions across page reloads

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are reducers in redux?

The **reducer** is a _pure function_ that takes the previous state and an action, and returns the next state.

```js
(previousState, action) => newState
```

It's called a reducer because it's the type of function you would pass to `Array.prototype.reduce(reducer, ?initialValue)`. It's very important that the reducer stays _pure_. Things you should never do inside a reducer:

* Mutate its arguments;
* Perform side effects like API calls and routing transitions;
* Call non-pure functions, e.g. `Date.now()` or `Math.random()`.

###### Source

* https://redux.js.org/basics/reducers

[[↑] Back to top](#Redux)
### What is Redux Thunk?

**Redux Thunk** middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods dispatch and `getState()` as parameters.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is the difference between React context and React redux?

You can use **Context** in your application directly and is going to be great for passing down data to deeply nested components which what it was designed for. Whereas **Redux** is much more powerful and provides a large number of features that the Context Api doesn't provide. 

Also, React Redux uses context internally but it doesn’t expose this fact in the public API. So you should feel much safer using context via React Redux than directly because if it changes, the burden of updating the code will be on React Redux instead developer responsibility.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is redux-saga?

**redux-saga** is a library that aims to make side effects (i.e. asynchronous things like data fetching and impure things like accessing the browser cache) in React/Redux applications easier and better.
It is available in NPM as

```sh
npm install --save redux-saga
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are the core principles of Redux?

Redux follows three fundamental principles:
1. **Single source of truth:** The state of your whole application is stored in an object tree within a single store. The single state tree makes it easier to keep track of changes over time and debug or inspect the application.
2. **State is ready only:** The only way to change the state is to emit an action, an object describing what happened. This ensures that neither the views nor the network callbacks will ever write directly to the state.
3. **Changes are made with pure functions:** To specify how the state tree is transformed by actions, you write pure reducers(Reducers are just pure functions that take the previous state and an action, and return the next state).

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How to set initial state in Redux?

You need to pass initial state as second argument to `createStore`
```js
const rootReducer = combineReducers({
  todos: todos,
  visibilityFilter: visibilityFilter
});

const initialState = {
  todos: [{id:123, name:'sudheer', completed: false}]
};

const store = createStore(
  rootReducer,
  initialState
);
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How to structure Redux top level directories?

Most of the applications has several top-level directories as below
1. **Components** Used for “dumb” React components unaware of Redux
2. **Containers** Used for “smart” React components connected to Redux
3. **Actions** Used for all action creators, where file name corresponds to part of the app
4. **Reducers** Used for all reducers, where file name corresponds to state key
5. **Store** Used for store initialization
This structure works well for small and mid-level size apps.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are the downsides of Redux over Flux?

Instead of saying downsides we can say that there are few compromises of using Redux over Flux. Those are as follows:
1. **You will need to learn avoiding mutations:**
Flux is un-opinionated about mutating data, but Redux doesn't like mutations and many packages complementary to Redux assume you never mutate the state. You can enforce this with dev-only packages like redux-immutable-state-invariant, Immutable.js, or your team to write non-mutative code.
2. **You're going to have to carefully pick your packages:**
While Flux explicitly doesn't try to solve problems such as undo/redo, persistence, or forms, Redux has extension points such as middleware and store enhancers, and it has spawned a young but rich ecosystem. This means most packages are new ideas and haven't received the critical mass of usage yet
3. **There is no nice Flow integration yet:**
Flux currently lets you do very impressive static type checks which Redux doesn't support yet.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are the differences between redux-saga and redux-thunk?

Both **Redux Thunk** and **Redux Saga** take care of dealing with side effects. In most of the scenarios, Thunk allows _Promises_ to deal with them, whereas Saga uses _Generators_. 

Thunk is simple to use and Promises are familiar to many developers, Saga/Generators are more powerful but you will need to learn them. But both the two middleware can coexists, so you can start with Thunks and introduce Sagas when/if you need them.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is the purpose of the constants in Redux?

Constants allow you to easily find all usages of that specific functionality across the project when you use an IDE. It also prevents you from introducing silly bugs caused by typos -- in which case, you will get a ReferenceError immediately.

Normally we will save them in a single file (constants.js or actionTypes.js)
For example:
```js
export const ADD_TODO = 'ADD_TODO';
export const DELETE_TODO = 'DELETE_TODO';
export const EDIT_TODO = 'EDIT_TODO';
export const COMPLETE_TODO = 'COMPLETE_TODO';
export const COMPLETE_ALL = 'COMPLETE_ALL';
export const CLEAR_COMPLETED = 'CLEAR_COMPLETED';
```
In redux you use them in two places
1. **During actions creation**
Let's take actions.js

```js
import { ADD_TODO } from './actionTypes';

export function addTodo(text) {
  return { type: ADD_TODO, text };
}
```
2. **Reducers**
Let's create reducer.js

```js
import { ADD_TODO } from './actionTypes';

export default (state = [], action) => {
  switch (action.type) {
    case ADD_TODO:
      return [
        ...state,
        {
          text: action.text,
          completed: false
        }
      ];
    default:
      return state
  }
};
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How to use connect from react redux?

You need to follow two steps to use your store in your container
1. **Use mapStateToProps():** It maps the state variables from your store to the props that you specify
2. **Connect the above props to your container:** The object returned by the mapStateToProps component is connected to the container. You can import connect from react-redux like 

```js
import React from 'react';
import { connect } from 'react-redux';

 class App extends React.Component {
   render() {
     return <div>{this.props.containerData}</div>;
   }
 }

 function mapStateToProps(state) {
   return { containerData: state.appData };
 }

 export default connect(mapStateToProps)(App);

function mapStateToProps(state) {
  return { containerData: state.data };
}

export default connect(mapStateToProps)(App);
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### Are there any similarities between Redux and RxJS?

These libraries are very different for very different purposes, but there are some vague similarities.

* **Redux** is a tool for managing state throughout the application. It is usually used as an architecture for UIs. Think of it as an alternative to (half of) Angular. 

* **RxJS** is a reactive programming library. It is usually used as a tool to accomplish asynchronous tasks in JavaScript. Think of it as an alternative to Promises. 

Redux uses the Reactive paradigm little bit because the Store is reactive. The Store observes actions from a distance, and changes itself. RxJS also uses the Reactive paradigm, but instead of being an architecture, it gives you basic building blocks, Observables, to accomplish this "observing from a distance" pattern.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is Redux form?

**Redux Form** works with React and Redux to enable a form in React to use Redux to store all of its state. Redux Form can be used with raw HTML5 inputs, but it also works with very well with common UI frameworks like Material UI, React Widgets and React Bootstrap.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are the main features of Redux Form?

Below are the major features of redux form:
1. Field values persistence via Redux store
2. Validation (sync/async) and submission
3. Formatting, parsing and normalization of field values

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How to access redux store outside a react component?

Yes.You just need to export the store from the module where it created with `createStore`. Also, it shouldn't pollute the global window object
```js
store = createStore(myReducer);
export default store;
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is the proper way to access Redux store?

The best way to access your store through a component is using the `connect()` function. Actually creates a new component that wraps around your existing one! This pattern is called _Higher-Order Components_, and is generally the preferred way of extending a component's functionality in React. This allows you to map state and action creators to your component, and have them passed in automatically as your store updates. Let's take an example of `FilterLink` component using connect,
```js
import { connect } from 'react-redux'
import { setVisibilityFilter } from '../actions'
import Link from '../components/Link'

const mapStateToProps = (state, ownProps) => {
  return {
    active: ownProps.filter === state.visibilityFilter
  }
}

const mapDispatchToProps = (dispatch, ownProps) => {
  return {
    onClick: () => {
      dispatch(setVisibilityFilter(ownProps.filter))
    }
  }
}

const FilterLink = connect(
  mapStateToProps,
  mapDispatchToProps
)(Link)

export default FilterLink
```
Due to it having quite a few performance optimizations and generally being less likely to cause bugs, the Redux devs almost always recommend using connect over accessing the store directly (using context API).
```js
class MyComponent {
  someMethod() {
    doSomethingWith(this.context.store);
  }
}
```


###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What are the differences between call and put in redux-saga?

Both **call** and **put** are effects creators functions. 

* **call** function is used to create effect description, which instructs middleware to call the promise. 
* **put** function creates effect, in which instructs middleware to dispatch an action to the store.

Let's take example of how these effects work for fetching particular user data

```js
function* fetchUserSaga(action) {
  // `call` function accepts rest arguments, which will be passed to `api.fetchUser` function.
  // Instructing middleware to call promise, it resolved value will be assigned to `userData` variable
  const userData = yield call(api.fetchUser, action.userId);
  // Instructing middleware to dispatch corresponding action.
  yield put({
    type: 'FETCH_USER_SUCCESS',
    userData
  });
}
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### Whats the purpose of at (@) symbol in the redux connect decorator?

The `@` symbol is in fact a JavaScript expression used to signify decorators. Decorators make it possible to annotate and modify classes and properties at design time. Let's take an example setting up Redux without and with a decorator

**Without decorator**
```js
import React from 'react';
import * as actionCreators from './actionCreators';
import { bindActionCreators } from 'redux';
import { connect } from 'react-redux';

function mapStateToProps(state) {
  return { todos: state.todos };
}

function mapDispatchToProps(dispatch) {
  return { actions: bindActionCreators(actionCreators, dispatch) };
}

class MyApp extends React.Component {
  // ...define your main app here
}

export default connect(mapStateToProps, mapDispatchToProps)(MyApp);
```
**With decorator**
```js
import React from 'react';
import * as actionCreators from './actionCreators';
import { bindActionCreators } from 'redux';
import { connect } from 'react-redux';

function mapStateToProps(state) {
  return { todos: state.todos };
}

function mapDispatchToProps(dispatch) {
  return { actions: bindActionCreators(actionCreators, dispatch) };
}

@connect(mapStateToProps, mapDispatchToProps)
export default class MyApp extends React.Component {
  // ...define your main app here
}
```
The above examples are almost similar except the usage of decorator. The decorator syntax isn't built into any Javascript runtimes yet, and is still experimental and subject to change. You can use babel for the decorators support.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How to make Ajax request in Redux?

You can use **redux-thunk** middleware which allows you to define async actions. Let's take an example of fetching specific account as a ajax call using fetch API,
```js
export function fetchAccount(id) {
 return dispatch => {
   dispatch(setLoadingAccountState()); // Show a loading spinner
   fetch(`/account/${id}`, (response) => {
     dispatch(doneFetchingAccount()); // Hide loading spinner
     if (response.status == 200){
       dispatch(setAccount(response.json)); // Use a normal function to set the received state
     } else {
       dispatch(someError)
     }
   })
 }
}

function setAccount(data) {
   return { type: 'SET_Account', data: data };
}
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### Why are Redux state functions called as reducers?

**Reducers** always return the accumulation of the state (based on all previous and current actions) not only default values. Therefore, they act as a reducer of state. Each time a redux reducer is called, the state is passed in with the action (state, action). This state is then reduced (or accumulated) based on the action, and then the next state is returned. i.e, You could "reduce" a collection of actions and an initial state (of the store) on which to perform these actions to get the resulting final state.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How to reset state in redux?

You need to write a root reducer in your application which delegate handling the action to the reducer generated by `combineReducers()`. For example, let us take rootReducer to return the initial state after `USER_LOGOUT` action. As we know, reducers are supposed to return the initial state when they are called with undefined as the first argument, no matter the action.

```js
const appReducer = combineReducers({
  /* your app’s top-level reducers */
})

const rootReducer = (state, action) => {
  if (action.type === 'USER_LOGOUT') {
    state = undefined
  }

  return appReducer(state, action)
}
```
In case of using redux-persist, you may also need to clean your storage. Redux-perist keeps a copy of your state in a storage engine. First, you need to import the appropriate storage engine and then, to parse the state before setting it to undefined and clean each storage state key,

```js
const appReducer = combineReducers({
  /* your app’s top-level reducers */
})

const rootReducer = (state, action) => {
  if (action.type === 'USER_LOGOUT') {
    Object.keys(state).forEach(key => {
                storage.removeItem(`persist:${key}`);
            });
            state = undefined;
  }

  return appReducer(state, action)
}
```

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### What is the mental model of redux-saga?

The mental model is that a saga is like a separate thread in your application that's solely responsible for side effects. redux-saga is a redux middleware, which means this thread can be started, paused and cancelled from the main application with normal redux actions, it has access to the full redux application state and it can dispatch redux actions as well.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
### How Relay is different from Redux?

**Relay** is similar to redux in that they both use a single store. The main difference is that relay only manages state originated from the server, and all access to the state is used via GraphQL queries (for reading data) and mutations (for changing data). Relay caches the data for you and optimizes data fetching for you, by fetching only changed data and nothing more.

###### Source

* https://github.com/sudheerj/reactjs-interview-questions

[[↑] Back to top](#Redux)
