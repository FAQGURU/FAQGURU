## Node.js

[What is Node.js?](#what-is-nodejs)

[What is npm?](#what-is-npm)

[What are the two types of API functions in Node.js? ](#what-are-the-two-types-of-api-functions-in-nodejs-)

[What are Event Listeners?  ](#what-are-event-listeners--)

[What is global installation of dependencies?](#what-is-global-installation-of-dependencies)

[What are the core modules of Node,js?](#what-are-the-core-modules-of-nodejs)

[What is an error-first callback?](#what-is-an-error-first-callback)

[ How you can monitor a file for modifications in Node.js ?](#-how-you-can-monitor-a-file-for-modifications-in-nodejs-)

[Could we run an external process with Node.js?](#could-we-run-an-external-process-with-nodejs)

[What's the difference between operational and programmer errors?](#whats-the-difference-between-operational-and-programmer-errors)

[What are the benefits of using Node.js?](#what-are-the-benefits-of-using-nodejs)

[What is the difference between Nodejs, AJAX, and jQuery?](#what-is-the-difference-between-nodejs-ajax-and-jquery)

[How to make Post request in Node.js?](#how-to-make-post-request-in-nodejs)

[What is Callback Hell?](#what-is-callback-hell)

[If Node.js is single threaded then how it handles concurrency?](#if-nodejs-is-single-threaded-then-how-it-handles-concurrency)

[What do you mean by Asynchronous API?](#what-do-you-mean-by-asynchronous-api)

[What are the key features of Node.js?](#what-are-the-key-features-of-nodejs)

[What is control flow function?  ](#what-is-control-flow-function--)

[Is Node a single threaded application?](#is-node-a-single-threaded-application)

[ List out the differences between AngularJS and NodeJS?](#-list-out-the-differences-between-angularjs-and-nodejs)

[What is the purpose of setTimeout function?](#what-is-the-purpose-of-settimeout-function)

[What is REPL in context of Node?](#what-is-repl-in-context-of-node)

[How can you avoid callback hells?](#how-can-you-avoid-callback-hells)

[What is Callback?](#what-is-callback)

[What's the event loop?](#whats-the-event-loop)

[What is a blocking code?](#what-is-a-blocking-code)

[How Node prevents blocking code?](#how-node-prevents-blocking-code)

[What is Event Loop?](#what-is-event-loop)

[What is stream and what are types of streams available in Node.js?](#what-is-stream-and-what-are-types-of-streams-available-in-nodejs)

[What is Event Emmitter?](#what-is-event-emmitter)

[How to avoid callback hell in Node.js?](#how-to-avoid-callback-hell-in-nodejs)

[What is purpose of Buffer class in Node?](#what-is-purpose-of-buffer-class-in-node)

[When should I use EventEmitter?](#when-should-i-use-eventemitter)

[What is difference between synchronous and asynchronous method of fs module?](#what-is-difference-between-synchronous-and-asynchronous-method-of-fs-module)

[What are streams?](#what-are-streams)

[What is the preferred method of resolving unhandled exceptions in Node.js?](#what-is-the-preferred-method-of-resolving-unhandled-exceptions-in-nodejs)

[When should we use Node.js?](#when-should-we-use-nodejs)

[How to use Buffer in Node.js?](#how-to-use-buffer-in-nodejs)

[What is Chaining in Node?](#what-is-chaining-in-node)

[What are the global objects of Node.js?](#what-are-the-global-objects-of-nodejs)

[Explain how does Node.js work?](#explain-how-does-nodejs-work)

[How does Node.js handle child threads?](#how-does-nodejs-handle-child-threads)

[How can you listen on port 80 with Node?](#how-can-you-listen-on-port-80-with-node)

[When to not use Node.js?](#when-to-not-use-nodejs)

[Is Node.js entirely based on a single-thread?](#is-nodejs-entirely-based-on-a-single-thread)

[Does Node.js support multi-core platforms? And is it capable of utilizing all the cores?](#does-nodejs-support-multi-core-platforms-and-is-it-capable-of-utilizing-all-the-cores)

[Why to use Buffers instead of binary strings to handle binary data ?](#why-to-use-buffers-instead-of-binary-strings-to-handle-binary-data-)

[What's a stub? Name a use case.](#whats-a-stub-name-a-use-case)

[What tools can be used to assure consistent code style?](#what-tools-can-be-used-to-assure-consistent-code-style)

[How to gracefully Shutdown Node.js Server?](#how-to-gracefully-shutdown-nodejs-server)

[Is Node.js entirely based on a single-thread?](#is-nodejs-entirely-based-on-a-single-thread)

[What is the purpose of __dirname variable?](#what-is-the-purpose-of-__dirname-variable)

[What is the purpose of __filename variable?](#what-is-the-purpose-of-__filename-variable)

[What are the timing features of Node.js?](#what-are-the-timing-features-of-nodejs)

[Name some of the events fired by streams.](#name-some-of-the-events-fired-by-streams)

[What is Piping in Node?](#what-is-piping-in-node)

[Explain usage of NODE_ENV](#explain-usage-of-node_env)

[Provide some example of config file separation for dev and prod environments](#provide-some-example-of-config-file-separation-for-dev-and-prod-environments)

[How would you handle errors for async code in Node.js?](#how-would-you-handle-errors-for-async-code-in-nodejs)

[Explain what is Reactor Pattern in Node.js?](#explain-what-is-reactor-pattern-in-nodejs)

[Rewrite the code sample without try/catch block](#rewrite-the-code-sample-without-trycatch-block)

[Consider following code snippet](#consider-following-code-snippet)

[Explain some Error Handling approaches in Node.js you know about. Which one will you use?](#explain-some-error-handling-approaches-in-nodejs-you-know-about-which-one-will-you-use)

[How would you scale Node application?](#how-would-you-scale-node-application)

[What is LTS releases of Node.js why should you care?](#what-is-lts-releases-of-nodejs-why-should-you-care)

[Why should you separate Express 'app' and 'server'?](#why-should-you-separate-express-app-and-server)

[Can Node.js use other engines than V8?](#can-nodejs-use-other-engines-than-v8)

[What is the difference between process.nextTick() and setImmediate() ?](#what-is-the-difference-between-processnexttick-and-setimmediate-)

[How to solve "Process out of Memory Exception" in Node.js ?](#how-to-solve-process-out-of-memory-exception-in-nodejs-)



### What is Node.js?

Node.js is a web application framework built on Google Chrome's JavaScript Engine (V8 Engine).

Node.js comes with runtime environment on which a Javascript based script can be interpreted and executed (It is analogus to JVM to JAVA byte code). This runtime allows to execute a JavaScript code on any machine outside a browser. Because of this runtime of Node.js, JavaScript is now can be executed on server as well.

*Node.js = Runtime Environment + JavaScript Library*

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is npm?

`npm` stands for Node Package Manager. npm provides following two main functionalities:

*   Online repositories for node.js packages/modules which are searchable on [search.nodejs.org](http://search.nodejs.org)
*   Command line utility to install packages, do version management and dependency management of Node.js packages.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What are the two types of API functions in Node.js? 

The two types of API functions in Node.js are: a) Asynchronous, non-blocking functions b) Synchronous, blocking functions

###### Source

* http://www.lazyquestion.com/interview-questions-and-answer/nodejs

[[↑] Back to top](#Nodejs)
### What are Event Listeners?  

**Event Listeners** are similar to call back functions but are associated with some event. For example when a server listens to http request on a given port a event will be generated and to specify http server has received and will invoke corresponding event listener. Basically, Event listener's are also call backs for a corresponding event.

Node.js has built in event's and built in event listeners. Node.js also provides functionality to create Custom events and Custom Event listeners.

###### Source

* http://www.lazyquestion.com/interview-questions-and-answer/nodejs?page=3

[[↑] Back to top](#Nodejs)
### What is global installation of dependencies?

Globally installed packages/dependencies are stored in **<user-directory>**/npm directory. Such dependencies can be used in CLI (Command Line Interface) function of any node.js but can not be imported using require() in Node application directly. To install a Node project globally use -g flag.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What are the core modules of Node,js?

* EventEmitter
* Stream
* FS
* Net
* Global Objects

###### Source

* https://github.com/jimuyouyou/node-interview-questions

[[↑] Back to top](#Nodejs)
### What is an error-first callback?

*Error-first callbacks* are used to pass errors and data. The first argument is always an error object that the programmer has to check if something went wrong. Additional arguments are used to pass data.

```js
fs.readFile(filePath, function(err, data) {
  if (err) {
    //handle the error
  }
  // use the data object
});
```

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
###  How you can monitor a file for modifications in Node.js ?

We can take advantage of File System `watch()` function which watches the changes of the file.

###### Source

* https://www.codingdefined.com/2017/04/top-20-interview-questions-on-nodejs.html

[[↑] Back to top](#Nodejs)
### Could we run an external process with Node.js?

Yes. *Child process module* enables us to access operating system functionaries or other apps. Scalability is baked into Node and child processes are the key factors to scale our application. You can use child process to run system commands, read large files without blocking event loop,  decompose the application into various “nodes” (That’s why it’s called Node).

Child process module has following three major ways to create child processes –

* spawn  - child_process.spawn launches a new process with a given command.
* exec  - child_process.exec method runs a command in a shell/console and buffers the output.
* fork - The child_process.fork method is a special case of the spawn() to create child processes.

###### Source

* https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/

[[↑] Back to top](#Nodejs)
### What's the difference between operational and programmer errors?

Operation errors are not bugs, but problems with the system, like _request timeout_ or _hardware failure_. On the other hand programmer errors are actual bugs.

###### Source

* https://blog.risingstack.com/node-js-interview-questions/

[[↑] Back to top](#Nodejs)
### What are the benefits of using Node.js?

Following are main benefits of using Node.js

*   **Aynchronous and Event Driven**All APIs of Node.js library are aynchronous that is non-blocking. It essentially means a Node.js based server never waits for a API to return data. Server moves to next API after calling it and a notification mechanism of Events of Node.js helps server to get response from the previous API call.
*   **Very Fast** Being built on Google Chrome's V8 JavaScript Engine, Node.js library is very fast in code execution.
*   **Single Threaded but highly Scalable** \- Node.js uses a single threaded model with event looping. Event mechanism helps server to respond in a non-bloking ways and makes server highly scalable as opposed to traditional servers which create limited threads to handle requests. Node.js uses a single threaded program and same program can services much larger number of requests than traditional server like Apache HTTP Server.
*   **No Buffering** \- Node.js applications never buffer any data. These applications simply output the data in chunks.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is the difference between Nodejs, AJAX, and jQuery?

The one common trait between Node.js, AJAX, and jQuery is that all of them are the advanced implementation of JavaScript. However, they serve completely different purposes.

* Node.js –It is a server-side platform for developing client-server applications. For example, if we’ve to build an online employee management system, then we won’t do it using client-side JS. But the Node.js can certainly do it as it runs on a server similar to Apache, Django not in a browser.

* AJAX (aka Asynchronous Javascript and XML) –It is a client-side scripting technique, primarily designed for rendering the contents of a page without refreshing it. There are a no. of large companies utilizing AJAX such as Facebook and Stack Overflow to display dynamic content.

* jQuery –It is a famous JavaScript module which complements AJAX, DOM traversal, looping and so on. This library provides many useful functions to help in JavaScript development. However, it’s not mandatory to use it but as it also manages cross-browser compatibility, so can help you produce highly maintainable web applications.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### How to make Post request in Node.js?

Following code snippet can be used to make a Post Request in Node.js.

```js
var request = require('request');
request.post('http://www.example.com/action', {
  form: {
    key: 'value'
  }
}, function(error, response, body) {
  if (!error && response.statusCode == 200) {
    console.log(body)
  }
});
```

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### What is Callback Hell?

The asynchronous function requires callbacks as a return parameter. When multiple asynchronous functions are chained together then callback hell situation comes up. 

###### Source

* https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/

[[↑] Back to top](#Nodejs)
### If Node.js is single threaded then how it handles concurrency?

Node provides a single thread to programmers so that code can be written easily and without bottleneck. Node internally uses multiple POSIX threads for various I/O operations such as File, DNS, Network calls etc.

When Node gets I/O request it creates or uses a thread to perform that I/O operation and once the operation is done, it pushes the result to the event queue. On each such event, event loop runs and checks the queue and if the execution stack of Node is empty then it adds the queue result to execution stack.

This is how Node manages concurrency.

###### Source

* https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/

[[↑] Back to top](#Nodejs)
### What do you mean by Asynchronous API?

All APIs of Node.js library are aynchronous that is non-blocking. It essentially means a Node.js based server never waits for a API to return data. Server moves to next API after calling it and a notification mechanism of Events of Node.js helps server to get response from the previous API call.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What are the key features of Node.js?

Let’s look at some of the key features of Node.js.

*   **Asynchronous event driven IO helps concurrent request handling –** All APIs of Node.js are asynchronous. This feature means that if a Node receives a request for some Input/Output operation, it will execute that operation in the background and continue with the processing of other requests. Thus it will not wait for the response from the previous requests.
*   **Fast in Code execution –** Node.js uses the V8 JavaScript Runtime engine, the one which is used by Google Chrome. Node has a wrapper over the JavaScript engine which makes the runtime engine much faster and hence processing of requests within Node.js also become faster.
*   **Single Threaded but Highly Scalable –** Node.js uses a single thread model for event looping. The response from these events may or may not reach the server immediately. However, this does not block other operations. Thus making Node.js highly scalable. Traditional servers create limited threads to handle requests while Node.js creates a single thread that provides service to much larger numbers of such requests.
*   **Node.js library uses JavaScript –** This is another important aspect of Node.js from the developer’s point of view. The majority of developers are already well-versed in JavaScript. Hence, development in Node.js becomes easier for a developer who knows JavaScript.
*   **There is an Active and vibrant community for the Node.js framework –** The active community always keeps the framework updated with the latest trends in the web development.
*   **No Buffering –** Node.js applications never buffer any data. They simply output the data in chunks.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### What is control flow function?  

It is a generic piece of code which runs in between several asynchronous function calls is known as control flow function.

###### Source

* http://www.lazyquestion.com/interview-questions-and-answer/nodejs

[[↑] Back to top](#Nodejs)
### Is Node a single threaded application?

Yes! Node uses a single threaded model with event looping.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
###  List out the differences between AngularJS and NodeJS?

AngularJS is a web application development framework. It’s a JavaScript and it is different from other web app frameworks written in JavaScript like jQuery. NodeJS is a runtime environment used for building server-side applications while AngularJS is a JavaScript framework mainly useful in building/developing client-side part of applications which run inside a web browser.

###### Source

* http://a4academics.com/interview-questions/79-web/802-nodejs-interview?showall=&start=2

[[↑] Back to top](#Nodejs)
### What is the purpose of setTimeout function?

The `setTimeout(cb, ms)` global function is used to run callback `cb` after at least `ms` milliseconds. The actual delay depends on external factors like OS timer granularity and system load. A timer cannot span more than 24.8 days.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is REPL in context of Node?

**REPL** stands for Read Eval Print Loop and it represents a computer environment like a window console or unix/linux shell where a command is entered and system responds with an output. Node.js or Node comes bundled with a REPL environment. It performs the following desired tasks.

*   **Read** \- Reads user's input, parse the input into JavaScript data-structure and stores in memory.
*   **Eval** \- Takes and evaluates the data structure
*   **Print** \- Prints the result
*   **Loop** \- Loops the above command until user press ctrl-c twice.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### How can you avoid callback hells?

To do so you have more options:

*   **modularization**: break callbacks into independent functions
*   use _Promises_
*   use `yield` with _Generators_ and/or _Promises_

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is Callback?

**Callback** is an asynchronous equivalent for a function. A callback function is called at the completion of a given task. Node makes heavy use of callbacks. All APIs of Node are written is such a way that they supports callbacks. 

For example, a function to read a file may start reading file and return the control to execution environment immediately so that next instruction can be executed. Once file I/O is complete, it will call the callback function while passing the callback function, the content of the file as parameter. So there is no blocking or wait for File I/O. 

This makes Node.js highly scalable, as it can process high number of request without waiting for any function to return result.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What's the event loop?

**The event loop** is what allows Node.js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded — by offloading operations to the system kernel whenever possible.

<div class="text-center">
<img src="https://i.stack.imgur.com/Lbs9z.png" class="img-fluid">
</div>

Every I/O requires a callback - once they are done they are pushed onto the event loop for execution. Since most modern kernels are multi-threaded, they can handle multiple operations executing in the background. When one of these operations completes, the kernel tells Node.js so that the appropriate callback may be added to the poll queue to eventually be executed.

###### Source

* https://blog.risingstack.com/node-js-interview-questions/

[[↑] Back to top](#Nodejs)
### What is a blocking code?

If application has to wait for some I/O operation in order to complete its execution any further then the code responsible for waiting is known as blocking code.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### How Node prevents blocking code?

By providing callback function. Callback function gets called whenever corresponding event triggered.


###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is Event Loop?

Node.js is a single threaded application but it support concurrency via concept of event and callbacks. As every API of Node js are asynchronous and being a single thread, it uses async function calls to maintain the concurrency. Node uses observer pattern. Node thread keeps an event loop and whenever any task get completed, it fires the corresponding event which signals the event listener function to get executed.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is stream and what are types of streams available in Node.js?

**Streams** are a collection of data that might not be available all at once and don’t have to fit in memory. Streams provide chunks of data in a continuous manner. It is useful to read a large set of data and process it.

There is four fundamental type of streams:

* Readable.
* Writeable.
* Duplex.
* Transform.

Readable streams as the name suggest used in reading a large chunk of data from a source. Writable streams are used in writing a large chunk of data to the destination.

Duplex streams are both readable and writable ( Eg socket). Transform stream is the duplex stream which is used in modifying the data (eg zip creation).

###### Source

* https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/

[[↑] Back to top](#Nodejs)
### What is Event Emmitter?

All objects that emit events are members of EventEmitter class. These objects expose an `eventEmitter.on()` function that allows one or more functions to be attached to named events emitted by the object.

When the EventEmitter object emits an event, all of the functions attached to that specific event are called synchronously. 

```js
const EventEmitter = require('events');

class MyEmitter extends EventEmitter {}

const myEmitter = new MyEmitter();
myEmitter.on('event', () => {
  console.log('an event occurred!');
});
myEmitter.emit('event');
```

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### How to avoid callback hell in Node.js?

Node.js internally uses a single-threaded event loop to process queued events. But this approach may lead to blocking the entire process if there is a task running longer than expected.

Node.js addresses this problem by incorporating callbacks also known as higher-order functions. So whenever a long-running process finishes its execution, it triggers the callback associated. 

sometimes, it could lead to complex and unreadable code. More the no. of callbacks, longer the chain of returning callbacks would be.

There are four solutions which can address the callback hell problem.

**Make your program modular**

It proposes to split the logic into smaller modules. And then join them together from the main module to achieve the desired result.

**Use async mechanism**

It is a widely used Node.js module which provides a sequential flow of execution.

The async module has <async.waterfall> API which passes data from one operation to other using the next callback.

Another async API <async.map> allows iterating over a list of items in parallel and calls back with another list of results.

With the async approach, the caller’s callback gets called only once. The caller here is the main method using the async module.

**Use promises mechanism**

Promises give an alternate way to write async code. They either return the result of execution or the error/exception. Implementing promises requires the use of <.then()> function which waits for the promise object to return. It takes two optional arguments, both functions. Depending on the state of the promise only one of them will get called. The first function call proceeds if the promise gets fulfilled. However, if the promise gets rejected, then the second function will get called.

**Use generators**

Generators are lightweight routines, they make a function wait and resume via the yield keyword. Generator functions uses a special syntax <function* ()>. They can also suspend and resume asynchronous operations using constructs such as promises or <thunks> and turn a synchronous code into asynchronous.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### What is purpose of Buffer class in Node?

**Buffer** class is a global class and can be accessed in application without importing buffer module. A Buffer is a kind of an array of integers and corresponds to a raw memory allocation outside the V8 heap. A Buffer cannot be resized.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### When should I use EventEmitter?

Whenever it makes sense for code to *subscribe* to something rather than get a callback from something. The typical use case would be that there's multiple blocks of code in your application that may need to do something when an event happens.

###### Source

* https://stackoverflow.com/questions/38881170/when-should-i-use-eventemitter

[[↑] Back to top](#Nodejs)
### What is difference between synchronous and asynchronous method of fs module?


Every method in `fs` module has synchronous as well as asynchronous form. Asynchronous methods takes a last parameter as completion function callback and first parameter of the callback function is error. It is preferred to use asynchronous method instead of synchronous method as former never block the program execution where the latter one does.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What are streams?

Streams are objects that let you read data from a source or write data to a destination in continuous fashion. In Node.js, there are four types of streams.

*   **Readable** \- Stream which is used for read operation.
*   **Writable** \- Stream which is used for write operation.
*   **Duplex** \- Stream which can be used for both read and write operation.
*   **Transform** \- A type of duplex stream where the output is computed based on input.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is the preferred method of resolving unhandled exceptions in Node.js?

Unhandled exceptions in Node.js can be caught at the `Process` level by attaching a handler for `uncaughtException` event.

```js
process.on('uncaughtException', function(err) {
  console.log('Caught exception: ' + err);
});
```
However, `uncaughtException` is a very crude mechanism for exception handling and may be removed from Node.js in the future. An exception that has bubbled all the way up to the `Process` level means that your application, and Node.js may be in an undefined state, and the only sensible approach would be to restart everything.

The preferred way is to add another layer between your application and the Node.js process which is called the [domain](http://nodejs.org/api/domain.html).

Domains provide a way to handle multiple different I/O operations as a single group. So, by having your application, or part of it, running in a separate domain, you can safely handle exceptions at the domain level, before they reach the `Process` level.

###### Source

* http://www.lazyquestion.com/interview-questions-and-answer/nodejs?page=3

[[↑] Back to top](#Nodejs)
### When should we use Node.js?

It’s ideal to use Node.js for developing streaming or event-based real-time applications that require less CPU usage such as.

*   Chat applications.
*   Game servers.

Node.js is good for fast and high-performance servers, that face the need to handle thousands of user requests simultaneously.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### How to use Buffer in Node.js?

Buffer is used to process binary data, such as pictures, mp3, database files, etc. Buffer supports a variety of encoding and decoding, binary string conversion.

###### Source

* https://github.com/jimuyouyou/node-interview-questions

[[↑] Back to top](#Nodejs)
### What is Chaining in Node?

**Chanining** is a mechanism to connect output of one stream to another stream and create a chain of multiple stream operations. It is normally used with piping operations.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What are the global objects of Node.js?

These objects are available in all modules:
* **process** - The process object is a global that provides information about, and control over, the current Node.js process. 
* **console** - Used to print to stdout and stderr. 
* **buffer** - Used to handle binary data. 

###### Source

* https://github.com/jimuyouyou/node-interview-questions

[[↑] Back to top](#Nodejs)
### Explain how does Node.js work?

A Node.js application creates a single thread on its invocation. Whenever Node.js receives a request, it first completes its processing before moving on to the next request.

Node.js works asynchronously by using the event loop and callback functions, to handle multiple requests coming in parallel. An Event Loop is a functionality which handles and processes all your external events and just converts them to a callback function. It invokes all the event handlers at a proper time. Thus, lots of work is done on the back-end, while processing a single request, so that the new incoming request doesn’t have to wait if the processing is not complete.

<img src="https://csharpcorner-mindcrackerinc.netdna-ssl.com/article/node-js-event-loop/Images/1.png" class="img-fluid"/>

While processing a request, Node.js attaches a callback function to it and moves it to the back-end. Now, whenever its response is ready, an event is called which triggers the associated callback function to send this response.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### How does Node.js handle child threads?

Node.js, in its essence, is a single thread process. It does not expose child threads and thread management methods to the developer. Technically, Node.js does spawn child threads for certain tasks such as asynchronous I/O, but these run behind the scenes and do not execute any application JavaScript code, nor block the main event loop.

If threading support is desired in a Node.js application, there are tools available to enable it, such as the ChildProcess module.

###### Source

* http://www.lazyquestion.com/interview-questions-and-answer/nodejs?page=3

[[↑] Back to top](#Nodejs)
### How can you listen on port 80 with Node?

Run the application on any port above 1024, then put a reverse proxy like [nginx](http://nginx.org/) in front of it.

###### Source

* https://blog.risingstack.com/node-js-interview-questions/

[[↑] Back to top](#Nodejs)
### When to not use Node.js?

We can use Node.js for a variety of applications. But it is a single threaded framework, so we should not use it for cases where the application requires long processing time. If the server is doing some calculation, it won’t be able to process any other requests. Hence, Node.js is best when processing needs less dedicated CPU time.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### Is Node.js entirely based on a single-thread?

Yes, it’s true that Node.js processes all requests on a single thread. But it’s just a part of the theory behind Node.js design. In fact, more than the single thread mechanism, it makes use of events and callbacks to handle a large no. of requests asynchronously.

Moreover, Node.js has an optimized design which utilizes both JavaScript and C++ to guarantee maximum performance. JavaScript executes at the server-side by Google Chrome v8 engine. And the C++ lib UV library takes care of the non-sequential I/O via background workers.

To explain it practically, let’s assume there are 100s of requests lined up in Node.js queue. As per design, the main thread of Node.js event loop will receive all of them and forwards to background workers for execution. Once the workers finish processing requests, the registered callbacks get notified on event loop thread to pass the result back to the user.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### Does Node.js support multi-core platforms? And is it capable of utilizing all the cores?

Yes, Node.js would run on a multi-core system without any issue. But it is by default a single-threaded application, so it can’t completely utilize the multi-core system.

However, Node.js can facilitate deployment on multi-core systems where it does use the additional hardware. It packages with a Cluster module which is capable of starting multiple Node.js worker processes that will share the same port.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### Why to use Buffers instead of binary strings to handle binary data ?

Pure JavaScript does not able to handle straight binary data very well. Since Node.js servers have to deal with TCP streams for reading and writing of data, binary strings will become problematic to work with as it is very slow and has a tendency to break. That's why it is always advisable to use Buffers instead of binary strings to handle binary data.

###### Source

* https://www.codingdefined.com/2017/04/top-20-interview-questions-on-nodejs.html

[[↑] Back to top](#Nodejs)
### What's a stub? Name a use case.

**Stubs** are functions/programs that simulate the behaviours of components/modules. Stubs provide canned answers to function calls made during test cases. Also, you can assert on with what these stubs were called.

A use-case can be a file read, when you do not want to read an actual file:

```js
var fs = require('fs');

var readFileStub = sinon.stub(fs, 'readFile', function(path, cb) {
  return cb(null, 'filecontent');
});

expect(readFileStub).to.be.called;
readFileStub.restore();
```

###### Source

* https://blog.risingstack.com/node-js-interview-questions/

[[↑] Back to top](#Nodejs)
### What tools can be used to assure consistent code style?

You have plenty of options to do so:

*   [JSLint](http://jslint.com/) by Douglas Crockford
*   [JSHint](http://jshint.com/)
*   [ESLint](http://eslint.org/)
*   [JSCS](http://jscs.info/)

These tools are really helpful when developing code in teams, to enforce a given style guide and to catch common errors using static analysis.

###### Source

* https://blog.risingstack.com/node-js-interview-questions/

[[↑] Back to top](#Nodejs)
### How to gracefully Shutdown Node.js Server?

We can gracefully shutdown Node.js server by using the generic signal called SIGTERM or SIGINT which is used for program termination. We need to call SIGTERM or SIGINT which will terminate the program and clean up the resources utilized by the program.

###### Source

* https://www.codingdefined.com/2017/04/top-20-interview-questions-on-nodejs.html

[[↑] Back to top](#Nodejs)
### Is Node.js entirely based on a single-thread?

Yes, it’s true that Node.js processes all requests on a single thread. But it’s just a part of the theory behind Node.js design. In fact, more than the single thread mechanism, it makes use of events and callbacks to handle a large no. of requests asynchronously.

Moreover, Node.js has an optimized design which utilizes both JavaScript and C++ to guarantee maximum performance. JavaScript executes at the server-side by Google Chrome v8 engine. And the C++ lib UV library takes care of the non-sequential I/O via background workers.

To explain it practically, let’s assume there are 100s of requests lined up in Node.js queue. As per design, the main thread of Node.js event loop will receive all of them and forwards to background workers for execution. Once the workers finish processing requests, the registered callbacks get notified on event loop thread to pass the result back to the user.

###### Source

* http://www.techbeamers.com/top-30-node-js-interview-questions-answers/

[[↑] Back to top](#Nodejs)
### What is the purpose of __dirname variable?

The `__dirname` represents the name of the directory that the currently executing script resides in.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is the purpose of __filename variable?

The `__filename` represents the filename of the code being executed. This is the resolved absolute path of this code file. For a main program this is not necessarily the same filename used in the command line. The value inside a module is the path to that module file.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What are the timing features of Node.js?

The Timers module in Node.js contains functions that execute code after a set period of time. 

* **setTimeout/clearTimeout** - can be used to schedule code execution after a designated amount of milliseconds
* **setInterval/clearInterval** - can be used to execute a block of code multiple times 
* **setImmediate/clearImmediate** - will execute code at the end of the current event loop cycle
* **process.nextTick** - used to schedule a callback function to be invoked in the next iteration of the Event Loop

```js
function cb(){
  console.log('Processed in next iteration');
}
process.nextTick(cb);
console.log('Processed in the first iteration');
```

Output:

```js
Processed in the first iteration
Processed in next iteration
```

###### Source

* https://github.com/jimuyouyou/node-interview-questions

[[↑] Back to top](#Nodejs)
### Name some of the events fired by streams.

Each type of Stream is an **EventEmitter** instance and throws several events at different instance of times. For example, some of the commonly used events are:

*   **data** \- This event is fired when there is data is available to read.
*   **end** \- This event is fired when there is no more data to read.
*   **error** \- This event is fired when there is any error receiving or writing data.
*   **finish** \- This event is fired when all data has been flushed to underlying system

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### What is Piping in Node?

**Piping** is a mechanism to connect output of one stream to another stream. It is normally used to get data from one stream and to pass output of that stream to another stream. There is no limit on piping operations.

###### Source

* http://www.tutorialspoint.com/nodejs/nodejs_interview_questions.htm

[[↑] Back to top](#Nodejs)
### Explain usage of NODE_ENV

Node encourages the convention of using a variable called NODE_ENV to flag whether we’re in production right now. This determination allows components to provide better diagnostics during development, for example by disabling caching or emitting verbose log statements. Setting NODE_ENV to production makes your application 3 times faster.

```sh
// Setting environment variables in bash before starting the node process
$ NODE_ENV=development
$ node

// Reading the environment variable using code
if (process.env.NODE_ENV === “production”)
    useCaching = true;
```

###### Source

* https://github.com/i0natan/nodebestpractices/blob/master/sections/production/setnodeenv.md

[[↑] Back to top](#Nodejs)
### Provide some example of config file separation for dev and prod environments

A perfect and flawless configuration setup should ensure:
* keys can be read from file AND from environment variable
* secrets are kept outside committed code
* config is hierarchical for easier findability

Consider the following config file:

```js
var config = {
  production: {
    mongo : {
      billing: '****'
    }
  },
  default: {
    mongo : {
      billing: '****'
    }
  }
}

exports.get = function get(env) {
  return config[env] || config.default;
}
```
And it's usage:
```js
const config = require('./config/config.js').get(process.env.NODE_ENV);
const dbconn = mongoose.createConnection(config.mongo.billing);
```

###### Source

* https://github.com/i0natan/nodebestpractices/blob/master/sections/projectstructre/configguide.md

[[↑] Back to top](#Nodejs)
### How would you handle errors for async code in Node.js?

Handling async errors in callback style (error-first approach) is probably the fastest way to hell (a.k.a the pyramid of doom). It's better to use a reputable promise library or async-await instead which enables a much more compact and familiar code syntax like try-catch.

Consider promises to catch errors:
```js
doWork()
 .then(doWork)
 .then(doOtherWork)
 .then((result) => doWork)
 .catch((error) => {throw error;})
 .then(verify);
```
or using async/await:
```js
async function check(req, res) {
    try {
        const a = await someOtherFunction();
        const b = await somethingElseFunction();
        res.send("result")
    } catch (error) {
        res.send(error.stack);
    }
}
```

###### Source

* https://github.com/i0natan/nodebestpractices/blob/master/sections/errorhandling/asyncerrorhandling.md

[[↑] Back to top](#Nodejs)
### Explain what is Reactor Pattern in Node.js?

**Reactor Pattern** is an idea of non-blocking I/O operations in Node.js. This pattern provides a handler(in case of Node.js, a *callback function*) that is associated with each I/O operation. When an I/O request is generated, it is submitted to a *demultiplexer*.

This *demultiplexer* is a notification interface that is used to handle concurrency in non-blocking I/O mode and collects every request in form of an event and queues each event in a queue. Thus, the demultiplexer provides the *Event Queue*. 

At the same time, there is an Event Loop which iterates over the items in the Event Queue. Every event has a callback function associated with it, and that callback function is invoked when the Event Loop iterates.

###### Source

* https://hackernoon.com/the-node-js-system-51090c35dddc

[[↑] Back to top](#Nodejs)
### Rewrite the code sample without try/catch block

```js
async function getData(){
  const a = await someFunction().catch((error)=>console.log(error));
  const b = await someOtherFunction().catch((error)=>console.log(error));
  if (a && b) console.log("some result")
}
```
or if you wish to know which specific function caused error:
```js
async function loginController() {
  try {
    const a = await loginService().
    catch((error) => {
      throw new CustomErrorHandler({
        code: 101,
        message: "a failed",
        error: error
      })
    });
    const b = await someUtil().
    catch((error) => {
      throw new CustomErrorHandler({
        code: 102,
        message: "b failed",
        error: error
      })
    });
    //someoeeoe
    if (a && b) console.log("no one failed")
  } catch (error) {
    if (!(error instanceof CustomErrorHandler)) {
      console.log("gen error", error)
    }
  }
}
```

###### Source

* https://medium.com/tech-buddy/async-await-without-try-catch-in-javascript-fdd38abf7e90

[[↑] Back to top](#Nodejs)
### Consider following code snippet

Within a web browser such as Chrome, declaring the variable `i` outside of any function’s scope makes it global and therefore binds it as a property of the `window` object. As a result, running this code in a web browser requires repeatedly resolving the property `i` within the heavily populated `window` namespace in each iteration of the `for` loop.

In Node.js, however, declaring any variable outside of any function’s scope binds it only to the module’s own scope (not the `window` object) which therefore makes it much easier and faster to resolve.

###### Source

* https://www.toptal.com/nodejs/interview-questions

[[↑] Back to top](#Nodejs)
### Explain some Error Handling approaches in Node.js you know about. Which one will you use?

Error handling in an asynchronous language works in a unique way and presents many challenges, some unexpected. There are four main error handling patterns in node:

* **Error return value** - doesn't work asynchronously

```js
var validateObject = function (obj) {
    if (typeof obj !== 'object') {
        return new Error('Invalid object');
    }
};
```
* **Error throwing** - well-establish pattern, in which a function does its thing and if an error situation arises, it simply bails out throwing an error. Can leave you in an unstable state. It requires extra work to catch them. Also wrapping the async calls in try/catch won't help because the errors happen asynchronously. To fix this, we need *domains*. Domains provide an asynchronous try...catch.

```js
var validateObject = function (obj) {
    if (typeof obj !== 'object') {
        throw new Error('Invalid object');
    }
};

try {
    validateObject('123');
}
catch (err) {
    console.log('Thrown: ' + err.message);
}
```
* **Error callback** - returning an error via a callback is the most common error handling pattern in Node.js. Handling error callbacks can become a mess (callback hell or the pyramid of doom).

```js
var validateObject = function (obj, callback) {
    if (typeof obj !== 'object') {
        return callback(new Error('Invalid object'));
    }
    return callback();
};

validateObject('123', function (err) {
    console.log('Callback: ' + err.message);
});
```
* **Error emitting** - when emitting errors, the errors are broadcast to any interested subscribers and handled within the same process tick, in the order subscribed.

```js
var Events = require('events');
var emitter = new Events.EventEmitter();

var validateObject = function (a) {
    if (typeof a !== 'object') {
        emitter.emit('error', new Error('Invalid object'));
    }
};

emitter.on('error', function (err) {
    console.log('Emitted: ' + err.message);
});

validateObject('123');
```
* **Promises** for async error handling

```js
doWork()
.then(doWork)
.then(doError)
.then(doWork)
.catch(errorHandler)
.then(verify);
```
* **Try...catch with async/await** - ES7 Async/await allows us as developers to write asynchronous JS code that look synchronous.

```js
async function f() {

  try {
    let response = await fetch('http://no-such-url');
  } catch(err) {
    alert(err); // TypeError: failed to fetch
  }
}

f();
```

* **Await-to-js lib** - async/await without try-catch blocks in Javascript

```js
import to from 'await-to-js';

async function main(callback) {
    const [err,quote] = await to(getQuote());

    if(err || !quote) return callback(new Error('No Quote found');

    callback(null,quote);

}
```

###### Source

* https://gist.github.com/hueniverse/5167027

[[↑] Back to top](#Nodejs)
### How would you scale Node application?

We can scale Node application in following ways:

* cloning using *Cluster* module.
* decomposing the application into smaller services – i.e micro services.

###### Source

* https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/

[[↑] Back to top](#Nodejs)
### What is LTS releases of Node.js why should you care?

An **LTS(Long Term Support)** version of Node.js receives all the critical bug fixes, security updates and performance improvements. 

LTS versions of Node.js are supported for at least 18 months and are indicated by even version numbers (e.g. 4, 6, 8). They're best for production since the LTS release line is focussed on stability and security, whereas the *Current* release line has a shorter lifespan and more frequent updates to the code. Changes to LTS versions are limited to bug fixes for stability, security updates, possible npm updates, documentation updates and certain performance improvements that can be demonstrated to not break existing applications.

###### Source

* https://github.com/i0natan/nodebestpractices/blob/master/sections/production/LTSrelease.md

[[↑] Back to top](#Nodejs)
### Why should you separate Express 'app' and 'server'?

Keeping the API declaration separated from the network related configuration (port, protocol, etc) allows testing the API in-process, without performing network calls, with all the benefits that it brings to the table: fast testing execution and getting coverage metrics of the code. It also allows deploying the same API under flexible and different network conditions. Bonus: better separation of concerns and cleaner code.

API declaration, should reside in app.js:

```js
var app = express();
app.use(bodyParser.json());
app.use("/api/events", events.API);
app.use("/api/forms", forms);
```
Server network declaration, should reside in /bin/www:

```js
var app = require('../app');
var http = require('http');

/**
 * Get port from environment and store in Express.
 */

var port = normalizePort(process.env.PORT || '3000');
app.set('port', port);

/**
 * Create HTTP server.
 */

var server = http.createServer(app);
```

###### Source

* https://github.com/i0natan/nodebestpractices/blob/master/sections/projectstructre/separateexpress.md

[[↑] Back to top](#Nodejs)
### Can Node.js use other engines than V8?

Yes. Microsoft Chakra is another JavaScript engine which can be used with Node.js. It’s not officially declared yet.

###### Source

* https://codeforgeek.com/2017/08/node-js-interview-questions-answers-updated/

[[↑] Back to top](#Nodejs)
### What is the difference between process.nextTick() and setImmediate() ?

The difference between `process.nextTick()` and `setImmediate()` is that `process.nextTick()` defers the execution of an action till the next pass around the event loop or it simply calls the callback function once the ongoing execution of the event loop is finished whereas `setImmediate()` executes a callback on the next cycle of the event loop and it gives back to the event loop for executing any I/O operations.

###### Source

* https://www.codingdefined.com/2017/04/top-20-interview-questions-on-nodejs.html

[[↑] Back to top](#Nodejs)
### How to solve "Process out of Memory Exception" in Node.js ?

To solve the process out of memory exception in Node.js we need to increase the `max-old-space-size`. By default the max size of max-old-space-size is 512 mb which you can increase by the command:

```sh
node --max-old-space-size=1024 file.js
```

###### Source

* https://www.codingdefined.com/2017/04/top-20-interview-questions-on-nodejs.html

[[↑] Back to top](#Nodejs)
