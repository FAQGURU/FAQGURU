## TypeScript

[What is TypeScript and why do we need it?](#what-is-typescript-and-why-do-we-need-it)

[What are Modules in Typescript?](#what-are-modules-in-typescript)

[ What is Typescript and why one should use it?](# what-is-typescript-and-why-one-should-use-it)

[Explain generics in TypeScript](#explain-generics-in-typescript)

[What is TypeScript and why would I use it in place of JavaScript?](#what-is-typescript-and-why-would-i-use-it-in-place-of-javascript)

[How to call base class constructor from child class in TypeScript?](#how-to-call-base-class-constructor-from-child-class-in-typescript)

[Do we need to compile TypeScript files and why?](#do-we-need-to-compile-typescript-files-and-why)

[List the built-in types in Typescript](#list-the-built-in-types-in-typescript)

[What are the benefits of TypeScript?](#what-are-the-benefits-of-typescript)

[What are the difference beetween Typescript and JavaScript?](#what-are-the-difference-beetween-typescript-and-javascript)

[What is Interface in TypeScript?](#what-is-interface-in-typescript)

[When to use interfaces and when to use classes in TypeScript?](#when-to-use-interfaces-and-when-to-use-classes-in-typescript)

[Which object oriented terms are supported by TypeScript?](#which-object-oriented-terms-are-supported-by-typescript)

[What is getters/setters in TypeScript?](#what-is-getterssetters-in-typescript)

[Does TypeScript support all object oriented principles?](#does-typescript-support-all-object-oriented-principles)

[How could you check null and undefined in TypeScript?](#how-could-you-check-null-and-undefined-in-typescript)

[How to implement class constants in TypeScript?](#how-to-implement-class-constants-in-typescript)

[Could we use TypeScript on backend and how?](#could-we-use-typescript-on-backend-and-how)

[What is the difference between Classes and Interfaces in Typescript?](#what-is-the-difference-between-classes-and-interfaces-in-typescript)

[What is "Decorators" in TypeScript?](#what-is-decorators-in-typescript)

[What is a TypeScript Map file?](#what-is-a-typescript-map-file)

[What's wrong with that code?](#whats-wrong-with-that-code)

[What are different components of TypeScript?](#what-are-different-components-of-typescript)

[Is that TypeScript code valid? Explain why.](#is-that-typescript-code-valid-explain-why)

[What is Typings in Typescript?](#what-is-typings-in-typescript)

[How To Use external plain JavaScript Libraries in TypeScript?](#how-to-use-external-plain-javascript-libraries-in-typescript)

[How TypeScript is optionally statically typed language?](#how-typescript-is-optionally-statically-typed-language)

[Are strongly-typed functions as parameters possible in TypeScript?](#are-strongly-typed-functions-as-parameters-possible-in-typescript)

[What is the default access modifier for members of a class in TypeScript?](#what-is-the-default-access-modifier-for-members-of-a-class-in-typescript)

[How can you allow classes defined in a module to accessible outside of the module?](#how-can-you-allow-classes-defined-in-a-module-to-accessible-outside-of-the-module)

[Explain how and why we could use property decorators in TS?](#explain-how-and-why-we-could-use-property-decorators-in-ts)

[Does TypeScript supports function overloading?](#does-typescript-supports-function-overloading)

[Explain why that code is marked as WRONG?](#explain-why-that-code-is-marked-as-wrong)

[What is the difference between "interface vs type" statements?](#what-is-the-difference-between-interface-vs-type-statements)

[How would you overload a class constructor in TypeScript?](#how-would-you-overload-a-class-constructor-in-typescript)

[What is one thing you would change about TypeScript?](#what-is-one-thing-you-would-change-about-typescript)

[Explain when to use "declare" keyword in TypeScript](#explain-when-to-use-declare-keyword-in-typescript)

[What are Ambients in TypeScripts and when to use them?](#what-are-ambients-in-typescripts-and-when-to-use-them)

[Is it possible to generate TypeScript declaration files from JS library?](#is-it-possible-to-generate-typescript-declaration-files-from-js-library)



### What is TypeScript and why do we need it?

JavaScript is the only client side language universally supported by all browsers. But JavaScript is not the best designed language. It’s not a class-based object-oriented language, doesn’t support class based inheritance, unreliable dynamic typing and lacks in compile time error checking. And TypeScript addresses all these problems. In other words, TypeScript is an attempt to “fix” JavaScript problems.

TypeScript is a free and open source programming language developed and maintained by Microsoft. It is a strict superset of JavaScript, and adds **optional static typing** and **class-based object-oriented programming** to the language. TypeScript is quite easy to learn and use for developers familiar with C#, Java and all strong typed languages. At the end of day “TypeScript is a language that generates plain JavaScript files.”

As stated on [Typescript official website](http://www.typescriptlang.org/), “TypeScript lets you write JavaScript the way you really want to. TypeScript is a typed superset of JavaScript that compiles to plain JavaScript. Any browser. Any host. Any OS. Open Source.” Where “**typed**” means that it considers the types of variables, parameters and functions.

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### What are Modules in Typescript?

Modules in Typescript helps in organizing the code. There are 2 types of Modules — Internal and External

* **Internal Modules** are now replaceable by using Typescript’s namespace.

* **External Modules** used to specify and load dependencies between multiple external js files. If there is only one js file used, then external modules are not relevant.



[[↑] Back to top](#TypeScript)
###  What is Typescript and why one should use it?

TypeScript is a free and open-source programming language developed and maintained by Microsoft. It is a strict syntactical superset of JavaScript, and adds optional static typing and class-based object-oriented programming to the language.



[[↑] Back to top](#TypeScript)
### Explain generics in TypeScript

Generics are able to create a component or function to work over a variety of types rather than a single one.

```js
/** A class definition with a generic parameter */
class Queue<T> {
  private data = [];
  push = (item: T) => this.data.push(item);
  pop = (): T => this.data.shift();
}

const queue = new Queue<number>();
queue.push(0);
queue.push("1"); // ERROR : cannot push a string. Only numbers allowed

```


###### Source

* https://basarat.gitbooks.io/typescript/docs/types/generics.html

[[↑] Back to top](#TypeScript)
### What is TypeScript and why would I use it in place of JavaScript?

**TypeScript** is a superset of JavaScript which primarily provides optional static typing, classes and interfaces. One of the big benefits is to enable IDEs to provide a richer environment for spotting common errors as *you type the code*. For a large JavaScript project, adopting TypeScript might result in more robust software, while still being deployable where a regular JavaScript application would run.

In details:
* TypeScript supports new ECMAScript standards and compiles them to (older) ECMAScript targets of your choosing. This means that you can use features of ES2015 and beyond, like modules, lambda functions, classes, the spread operator, destructuring, today. 
* JavaScript code is valid TypeScript code; TypeScript is a superset of JavaScript. 
* TypeScript adds type support to JavaScript. The type system of TypeScript is relatively rich and includes: interfaces, enums, hybrid types, generics, union and intersection types, access modifiers and much more. TypeScript makes typing a bit easier and a lot less explicit by the usage of type inference.
* The development experience with TypeScript is a great improvement over JavaScript. The IDE is informed in real-time by the TypeScript compiler on its rich type information. 
* With strict null checks enabled (`--strictNullChecks` compiler flag) the TypeScript compiler will not allow undefined to be assigned to a variable unless you explicitly declare it to be of nullable type. 
* To use TypeScript you need a build process to compile to JavaScript code. The TypeScript compiler can inline source map information in the generated .js files or create separate .map files. This makes it possible for you to set breakpoints and inspect variables during runtime directly on your TypeScript code. 
* TypeScript is open source (Apache 2 licensed, see github) and backed by Microsoft. *Anders Hejlsberg*, the lead architect of C# is spearheading the project.

###### Source

* https://stackoverflow.com/questions/12694530/what-is-typescript-and-why-would-i-use-it-in-place-of-javascript

[[↑] Back to top](#TypeScript)
### How to call base class constructor from child class in TypeScript?

We can call base class constructor using `super()`.

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### Do we need to compile TypeScript files and why?

Yes we do. Typescript is just a language Extension browsers can't interpret it. Converting from TypeScript to JavaScript is called compiling. Compiling doesn't mean binary code is created in this case. For this kind of translation, also the term transpilation is used instead of compilation.

###### Source

* https://stackoverflow.com/questions/45125284/why-is-angular-compiled

[[↑] Back to top](#TypeScript)
### List the built-in types in Typescript

These are also called the primitive types in TypeScript:
* **Number** type: it is used to represent number type values and represents double precision floating point values.
```js
var variable_name: number;
```
* **String** type: it represents a sequence of characters stored as Unicode UTF-16 code. It is the same as JavaScript primitive type.
```js
var variable_name: string;
```
* **Boolean** type: in Typescript, it is used to represent a logical value. When we use the Boolean type, we get output only in true or false. It is also the same as JavaScript primitive type.
```js
var variable_name: bool;
```
* **Null** type: it represents a null literal and it is not possible to directly reference the null type value itself.
```js
var variable_name:number = null;
```
* **Undefined** type: it is the type of undefined literal. This type of built-in type is the sub-type of all the types.
```js
var variable_name:number = undefined;
```




[[↑] Back to top](#TypeScript)
### What are the benefits of TypeScript?

TypeScript has following benefits.

*   It helps in code structuring.
*   Use class based object oriented programming.
*   Impose coding guidelines.
*   Offers type checking.
*   Compile time error checking.
*   Intellisense.

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### What are the difference beetween Typescript and JavaScript?

* It is an object oriented programming language (not pure).
* Here it is static typing (We can declare a variable in multiple ways). ex: var num : number.
* It has interfaces.
* It has optional parameter feature.
* It has Rest Parameter feature.
* Supports generics.
* Supports Modules
* Number, string etc. are the interfaces.




[[↑] Back to top](#TypeScript)
### What is Interface in TypeScript?

One of TypeScript’s core principles is that type-checking focuses on the *shape* that values have.

An `interface` is a virtual structure that only exists within the context of TypeScript. The TypeScript compiler uses interfaces solely for type-checking purposes.

When you define your interface you’re saying that any object (not an instance of a class) given this contract must be an object containing interfaces properties.

###### Source

* https://medium.com/front-end-hacking/typescript-class-vs-interface-99c0ae1c2136

[[↑] Back to top](#TypeScript)
### When to use interfaces and when to use classes in TypeScript?

If you need/wish to create an instance of perhaps a custom object, whilst getting the benefits of type-checking things such as arguments, return types or generics - a class makes sense. 

If you’re not creating instances - we have interfaces at our disposal, and their benefit comes from not generating any source code, yet allowing us to somewhat “virtually” type-check our code.

###### Source

* https://toddmotto.com/classes-vs-interfaces-in-typescript

[[↑] Back to top](#TypeScript)
### Which object oriented terms are supported by TypeScript?

TypeScript supports following object oriented terms:

*   Modules
*   Classes
*   Interfaces
*   Data Types
*   Member functions

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### What is getters/setters in TypeScript?

TypeScript supports **getters/setters** as a way of intercepting accesses to a member of an object. This gives you a way of having finer-grained control over how a member is accessed on each object.

```js
class foo {
  private _bar:boolean = false;

  get bar():boolean {
    return this._bar;
  }
  set bar(theBar:boolean) {
    this._bar = theBar;
  }
}

var myBar = myFoo.bar;  // correct (get)
myFoo.bar = true;  // correct (set)
```

###### Source

* http://www.typescriptlang.org/docs/handbook/classes.html

[[↑] Back to top](#TypeScript)
### Does TypeScript support all object oriented principles?

The answer is **YES**. There are 4 main principles to Object Oriented Programming: 

* Encapsulation, 
* Inheritance, 
* Abstraction, and 
* Polymorphism. 

TypeScript can implement all four of them with its smaller and cleaner syntax.

###### Source

* https://jonathanmh.com/typescript-node-js-tutorial-backend-beginner/

[[↑] Back to top](#TypeScript)
### How could you check null and undefined in TypeScript?

Just use:
```js
if (value) {
}
```
It will evaluate to `true` if `value` is not:

* `null`
* `undefined`
* `NaN`
* empty string `''`
* `0`
* `false`

TypesScript includes JavaScript rules.


###### Source

* https://stackoverflow.com/questions/28975896/is-there-a-dedicated-function-to-check-null-and-undefined-in-typescript

[[↑] Back to top](#TypeScript)
### How to implement class constants in TypeScript?

In TypeScript, the `const` keyword cannot be used to declare class properties. Doing so causes the compiler to an error with "A class member cannot have the 'const' keyword." TypeScript 2.0 has the `readonly` modifier:

```js
class MyClass {
    readonly myReadonlyProperty = 1;

    myMethod() {
        console.log(this.myReadonlyProperty);
    }
}

new MyClass().myReadonlyProperty = 5; // error, readonly
```

###### Source

* https://stackoverflow.com/questions/37265275/how-to-implement-class-constants-in-typescript

[[↑] Back to top](#TypeScript)
### Could we use TypeScript on backend and how?

Typescript doesn’t only work for browser or frontend code, you can also choose to write your backend applications. For example you could choose Node.js and have some additional type safety and the other abstraction that the language brings.

1. Install the default Typescript compiler  

```sh
npm i -g typescript
```
2. The TypeScript compiler takes options in the shape of a tsconfig.json file that determines where to put built files and in general is pretty similar to a babel or webpack config.

```sh
{
  "compilerOptions": {
    "target": "es5",
    "module": "commonjs",
    "declaration": true,
    "outDir": "build"
  }
}
```
3. Compile ts files

```sh
tsc
```
4. Run

```js
node build/index.js
```

###### Source

* https://jonathanmh.com/typescript-node-js-tutorial-backend-beginner/

[[↑] Back to top](#TypeScript)
### What is the difference between Classes and Interfaces in Typescript?

We use classes as object factories. A class defines a blueprint of what an object should look like and act like and then implements that blueprint by initialising class properties and defining methods. Classes are present throughout all the phases of our code.

Unlike classes, an interface is a virtual structure that only exists within the context of TypeScript. The TypeScript compiler uses interfaces solely for type-checking purposes. Once code is transpiled to its target language, it will be stripped from interfaces.

A class may define a factory or a singleton by providing initialisation to its properties and implementation to its methods, an interface is simply a structural contract that defines what the properties of an object should have as a name and as a type.

###### Source

* https://toddmotto.com/classes-vs-interfaces-in-typescript

[[↑] Back to top](#TypeScript)
### What is "Decorators" in TypeScript?

A *Decorator* is a special kind of declaration that can be attached to a class declaration, method, accessor, property, or parameter. Decorators are functions that take their target as the argument. With decorators we can run arbitrary code around the target execution or even entirely replace the target with a new definition.

There are 4 things we can decorate in ECMAScript2016 (and Typescript): constructors, methods, properties and parameters. 

###### Source

* https://www.sparkbit.pl/typescript-decorators/

[[↑] Back to top](#TypeScript)
### What is a TypeScript Map file?

`.map` files are source map files that let tools map between the emitted JavaScript code and the TypeScript source files that created it. Many debuggers (e.g. Visual Studio or Chrome's dev tools) can consume these files so you can debug the TypeScript file instead of the JavaScript file.

###### Source

* https://stackoverflow.com/questions/17493738/what-is-a-typescript-map-file

[[↑] Back to top](#TypeScript)
### What's wrong with that code?

Don’t ever use the types `Number`, `String`, `Boolean`, or `Object`. These types refer to non-primitive boxed objects that are almost never used appropriately in JavaScript code. Instead of Object, use the non-primitive `object` type. 

Consider:
```js
function reverse(s: string): string;
```

###### Source

* https://www.typescriptlang.org/docs/handbook/declaration-files/do-s-and-don-ts.html

[[↑] Back to top](#TypeScript)
### What are different components of TypeScript?

There are mainly 3 components of TypeScript .

1.  **Language** – The most important part for developers is the new language. The language consist of new syntax, keywords and allows you to write TypeScript.
2.  **Compiler** – The TypeScript compiler is open source, cross-platform and open specification, and is written in TypeScript. Compiler will compile your TypeScript into JavaScript. And it will also emit error, if any. It can also help in concating different files to single output file and in generating source maps.
3.  **Language Service** – TypeScript language service which powers the interactive TypeScript experience in Visual Studio, [VS Code](http://www.talkingdotnet.com/what-is-visual-studio-code-and-difference-between-visual-studio-2015/), Sublime, the TypeScript playground and other editor.

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### Is that TypeScript code valid? Explain why.

Yes, the code is valid. A class declaration creates two things: a *type* representing instances of the class and a *constructor function*. Because classes create types, you can use them in the same places you would be able to use interfaces.

###### Source

* http://www.typescriptlang.org/docs/handbook/classes.html

[[↑] Back to top](#TypeScript)
### What is Typings in Typescript?

TypeScript is mainly about adding types to JavaScript. When you use external libraries like jQuery or moment.js, there are no information of the types in that code. So in order to use it with TypeScript, you also have to get files that describe the types of that code. These are the type declaration files, most often with the file extension name `.d.ts`. Fortunately people have written those kinds of type declaration files for most common javascript libraries out there.

**Typings** was just a tool to install those files. It is now best practice to just use `npm`.

###### Source

* https://stackoverflow.com/questions/41573822/what-are-typings-in-typescript

[[↑] Back to top](#TypeScript)
### How To Use external plain JavaScript Libraries in TypeScript?

1. Include the library source file before the compiled TypeScript file 
2. In your TypeScript file before using the library, add

```js
declare var libGlobal: any;
```
3.  Use any library function just like normal .

###### Source

* https://stackoverflow.com/questions/17493738/what-is-a-typescript-map-file

[[↑] Back to top](#TypeScript)
### How TypeScript is optionally statically typed language?

TypeScript is referred as *optionally statically typed*, which means you can ask the compiler to ignore the type of a variable. Using `any` data type, we can assign any type of value to the variable. TypeScript will not give any error checking during compilation.

Consider:
```js
var unknownType: any = 4;
unknownType = "Okay, I am a string";
unknownType = false; // A boolean.
```

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### Are strongly-typed functions as parameters possible in TypeScript?


In TypeScript you can declare your **callback type** like:

```js
type NumberCallback = (n: number) => any;

class Foo {
    // Equivalent
    save(callback: NumberCallback): void {
        console.log(1)
        callback(42);
    }
}

var numCallback: NumberCallback = (result: number) : void => {
    console.log("numCallback: ", result.toString());
}

var foo = new Foo();
foo.save(numCallback)
```

###### Source

* https://stackoverflow.com/questions/12694530/what-is-typescript-and-why-would-i-use-it-in-place-of-javascript

[[↑] Back to top](#TypeScript)
### What is the default access modifier for members of a class in TypeScript?

In TypeScript, each member of class is **public** by default.

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### How can you allow classes defined in a module to accessible outside of the module?

Classes define in a module are available within the module. Outside the module you can’t access them.

```js
module Vehicle {
    class Car {
        constructor (
            public make: string, 
            public model: string) { }
    }
    var audiCar = new Car("Audi", "Q7");
}
// This won't work
var fordCar = Vehicle.Car("Ford", "Figo");
```

As per above code, `fordCar` variable will give us compile time error. To make classes accessible outside module use `export` keyword for classes.

```js
module Vehicle {
    export class Car {
        constructor (
            public make: string, 
            public model: string) { }
    }
    var audiCar = new Car("Audi", "Q7");
}
// This works now
var fordCar = Vehicle.Car("Ford", "Figo");
```

###### Source

* http://www.talkingdotnet.com/typescript-interview-questions/

[[↑] Back to top](#TypeScript)
### Explain how and why we could use property decorators in TS?

Decorators can be used to modify the behavior of a class or become even more powerful when integrated into a framework. For instance, if your framework has methods with restricted access requirements (just for admin), it would be easy to write an `@admin` method decorator to deny access to non-administrative users, or an `@owner` decorator to only allow the owner of an object the ability to modify it.

```ts
class CRUD {
    get() { }
    post() { }
 
    @admin
    delete() { }
 
    @owner
    put() { }
}
```

###### Source

* https://www.sitepen.com/blog/2015/10/20/typescript-decorators/

[[↑] Back to top](#TypeScript)
### Does TypeScript supports function overloading?

Yes, TypeScript does support function overloading but the implementation is a bit different if we compare it to OO languages. We are creating just one function and a number of declarations so that TypeScript doesn't give compile errors. When this code is compiled to JavaScript, the concrete function alone will be visible. As a JavaScript function can be called by passing multiple arguments, it just works.

```js
class Foo {
    myMethod(a: string);
    myMethod(a: number);
    myMethod(a: number, b: string);
    myMethod(a: any, b?: string) {
        alert(a.toString());
    }
}
```

###### Source

* https://www.typescriptlang.org/docs/handbook/declaration-files/do-s-and-don-ts.html

[[↑] Back to top](#TypeScript)
### Explain why that code is marked as WRONG?

Don’t use *optional parameters* in callbacks unless you really mean it. This code has a very specific meaning: the `done` callback might be invoked with 1 argument or might be invoked with 2 arguments. The author probably intended to say that the callback might not care about the `elapsedTime` parameter, but there’s no need to make the parameter optional to accomplish this – it’s always legal to provide a callback that accepts fewer arguments.

###### Source

* https://www.typescriptlang.org/docs/handbook/declaration-files/do-s-and-don-ts.html

[[↑] Back to top](#TypeScript)
### What is the difference between "interface vs type" statements?

Unlike an interface declaration, which always introduces a *named object type,* a type alias declaration can introduce a *name* for any kind of type, including primitive, union, and intersection types.

By using type instead of interface the following capabilities are lost:

* An interface can be named in an extends or implements clause, but a type alias for an object type literal cannot.
* An interface can have multiple merged declarations, but a type alias for an object type literal cannot.

###### Source

* https://stackoverflow.com/questions/37233735/typescript-interfaces-vs-types

[[↑] Back to top](#TypeScript)
### How would you overload a class constructor in TypeScript?

**TypeScript** allows you to declare overloads but you can only have one implementation and that implementation must have a signature that is compatible with all overloads. Some techniques for constructor overloading are:
* with an optional parameter as in

```ts
class Box {
    public x: number;
    public y: number;
    public height: number;
    public width: number;

    constructor();
    constructor(obj: IBox); 
    constructor(obj?: any) {    
        this.x = obj && obj.x || 0
        this.y = obj && obj.y || 0
        this.height = obj && obj.height || 0
        this.width = obj && obj.width || 0;
    }   
}
```
* default parameters

```ts
class Box {
    public x: number;
    public y: number;
    public height: number;
    public width: number;

    constructor(obj : IBox = {x:0,y:0, height:0, width:0}) {    
        this.x = obj.x;
        this.y = obj.y;
        this.height = obj.height;
        this.width = obj.width;
    }   
}
```
* additional overloads as static factory methods

```ts
class Person {
    static fromData(data: PersonData) {
        let { first, last, birthday, gender = 'M' } = data 
        return new this(
            `${last}, ${first}`,
            calculateAge(birthday),
            gender
        )
    }

    constructor(
        public fullName: string,
        public age: number,
        public gender: 'M' | 'F'
    ) {}
}

interface PersonData {
    first: string
    last: string
    birthday: string
    gender?: 'M' | 'F'
}


let personA = new Person('Doe, John', 31, 'M')
let personB = Person.fromData({
    first: 'John',
    last: 'Doe',
    birthday: '10-09-1986'
})
```
* using union types

```ts
class foo {
    private _name: any;
    constructor(name: string | number) {
        this._name = name;
    }
}
var f1 = new foo("bar");
var f2 = new foo(1);
```

###### Source

* https://stackoverflow.com/questions/12702548/constructor-overload-in-typescript

[[↑] Back to top](#TypeScript)
### What is one thing you would change about TypeScript?



###### Source

* https://www.reddit.com/r/typescript/comments/7rhlng/basic_typescript_interview_questions/

[[↑] Back to top](#TypeScript)
### Explain when to use "declare" keyword in TypeScript

The TypeScript `declare` keyword is used to declare variables that may not have originated from a TypeScript file. 

For example, lets imagine that we have a library called `myLibrary` that doesn’t have a TypeScript declaration file and have a namespace called `myLibrary` in the global namespace. If you want to use that library in your TypeScript code, you can use the following code:

```js
declare var myLibrary;
```
The type that the TypeScript runtime will give to `myLibrary` variable is the `any` type. The problem here is that you won’t have Intellisense for that variable in design time but you will be able to use the library in your code. Another option to have the same behavior without using the declare keyword is just using a variable with the any type:

```js
var myLibrary: any;
```

Both of the code examples will result in the same JavaScript output but the `declare` example is more readable and expresses an **ambient declaration**.

###### Source

* https://stackoverflow.com/questions/35019987/what-does-declare-do-in-export-declare-class-actions

[[↑] Back to top](#TypeScript)
### What are Ambients in TypeScripts and when to use them?

**Ambients** or **Ambient declarations** are a way of telling the TypeScript compiler that the actual source code exists elsewhere. Ambient declarations help to seamlessly integrate other js libraries into TypeScript.

Ambient declarations are by convention kept in a type declaration file with `d.ts` extension. The syntax for declaring ambient variables or modules will be as following:

```js
declare module Module_Name {
}
```
The ambient files should be referenced in the client TypeScript file as shown

```js
/// <reference path = " Sample.d.ts" />
```

###### Source

* https://stackoverflow.com/questions/35019987/what-does-declare-do-in-export-declare-class-actions

[[↑] Back to top](#TypeScript)
### Is it possible to generate TypeScript declaration files from JS library?

JavaScript doesn't always contain enough type information for the TypeScript compiler to infer the structures in your code - so automatically generating a definition based on JavaScript is rarely an option but:

* **Microsoft/dts-gen** - The official starting point Microsoft uses when creating types

* **dtsmake** - This one looks very promising. It depends on Ternjs which some editors use to provide autocomplete for JS code.


###### Source

* https://stackoverflow.com/questions/18301898/generating-typescript-declaration-files-from-javascript

[[↑] Back to top](#TypeScript)
