## Golang

[What is Go?](#what-is-go)

[Is Go a new language, framework or library?](#is-go-a-new-language-framework-or-library)

[What is static type declaration of a variable in Go?](#what-is-static-type-declaration-of-a-variable-in-go)

[What is dynamic type declaration of a variable in Go?](#what-is-dynamic-type-declaration-of-a-variable-in-go)

[Can you declared multiple types of variables in single declaration in Go?](#can-you-declared-multiple-types-of-variables-in-single-declaration-in-go)

[What is a pointer?](#what-is-a-pointer)

[Can you return multiple values from a function?](#can-you-return-multiple-values-from-a-function)

[What are some advantages of using Go?](#what-are-some-advantages-of-using-go)

[What kind of type conversion is supported by Go?](#what-kind-of-type-conversion-is-supported-by-go)

[What are the benefits of using Go programming?](#what-are-the-benefits-of-using-go-programming)

[Why the Go language was created?](#why-the-go-language-was-created)

[Does Go have exceptions?](#does-go-have-exceptions)

[What are Goroutines?](#what-are-goroutines)

[Let's talk variable declaration in Go. Could you explain what is a variable "zero value"?](#lets-talk-variable-declaration-in-go-could-you-explain-what-is-a-variable-zero-value)

[Is Go an object-oriented language?](#is-go-an-object-oriented-language)

[Name some advantages of Goroutines over threads](#name-some-advantages-of-goroutines-over-threads)

[Have you worked with Go 2?](#have-you-worked-with-go-2)

[What is "rune" type in Go?](#what-is-rune-type-in-go)

[What is so special about constants in Go?](#what-is-so-special-about-constants-in-go)



### What is Go?

**Go** is a general-purpose language designed with systems programming in mind. It was initially developed at Google in year 2007 by Robert Griesemer, Rob Pike, and Ken Thompson. It is strongly and statically typed, provides inbuilt support for garbage collection and supports concurrent programming. Programs are constructed using packages, for efficient management of dependencies. Go programming implementations use a traditional compile and link model to generate executable binaries.

###### Source

* https://www.tutorialspoint.com/go/go_interview_questions.htm

[[↑] Back to top](#Golang)
### Is Go a new language, framework or library?

**Go** isn't a library and not a framework, it's a new language. 

Go is mostly in the C family (basic syntax), with significant input from the Pascal/Modula/Oberon family (declarations, packages). Go does have an extensive library, called the runtime, that is part of every Go program. Although it is more central to the language, Go's runtime is analogous to libc, the C library. It is important to understand, however, that Go's runtime does not include a virtual machine, such as is provided by the Java runtime. Go programs are compiled ahead of time to native machine code.

###### Source

* https://golang.org/doc/faq

[[↑] Back to top](#Golang)
### What is static type declaration of a variable in Go?

*Static type variable declaration* provides assurance to the compiler that there is one variable existing with the given type and name so that compiler proceed for further compilation without needing complete detail about the variable. A variable declaration has its meaning at the time of compilation only, compiler needs actual variable declaration at the time of linking of the program.

###### Source

* https://www.tutorialspoint.com/go/go_interview_questions.htm

[[↑] Back to top](#Golang)
### What is dynamic type declaration of a variable in Go?

A *dynamic type variable declaration* requires compiler to interpret the type of variable based on value passed to it. Compiler don't need a variable to have type statically as a necessary requirement.

###### Source

* https://www.tutorialspoint.com/go/go_interview_questions.htm

[[↑] Back to top](#Golang)
### Can you declared multiple types of variables in single declaration in Go?

Yes. Variables of different types can be declared in one go using type inference.

```go
var a, b, c =  3,  4,  "foo"  
```

###### Source

* https://www.tutorialspoint.com/go/go_interview_questions.htm

[[↑] Back to top](#Golang)
### What is a pointer?

A **pointer variable** can hold the *address* of a variable.

Consider:
```go
var x =  5  var p *int p =  &x
fmt.Printf("x = %d",  *p)
```

Here `x` can be accessed by `*p`.

###### Source

* https://www.tutorialspoint.com/go/go_interview_questions.htm

[[↑] Back to top](#Golang)
### Can you return multiple values from a function?

A Go function can return multiple values.

Consider:
```go
package main
import "fmt"

func swap(x, y string) (string, string) {
   return y, x
}
func main() {
   a, b := swap("Mahesh", "Kumar")
   fmt.Println(a, b)
}
```

###### Source

* https://www.tutorialspoint.com/go/go_interview_questions.htm

[[↑] Back to top](#Golang)
### What are some advantages of using Go?

**Go** is an attempt to introduce a new, concurrent, garbage-collected language with fast compilation and the following benefits: 
* It is possible to compile a large Go program in a few seconds on a single computer.
* Go provides a model for software construction that makes dependency analysis easy and avoids much of the overhead of C-style include files and libraries.
* Go's type system has no hierarchy, so no time is spent defining the relationships between types. Also, although Go has static types, the language attempts to make types feel lighter weight than in typical OO languages.
* Go is fully garbage-collected and provides fundamental support for concurrent execution and communication.
* By its design, Go proposes an approach for the construction of system software on multicore machines.

###### Source

* https://golang.org/doc/faq

[[↑] Back to top](#Golang)
### What kind of type conversion is supported by Go?

Go is very strict about **explicit typing**. There is no automatic type promotion or conversion. Explicit type conversion is required to assign a variable of one type to another. 

Consider:
```go
i := 55      //int
j := 67.8    //float64
sum := i + int(j) //j is converted to int
```

###### Source

* https://golangbot.com/types/

[[↑] Back to top](#Golang)
### What are the benefits of using Go programming?

Following are the benefits of using Go programming:

*   Support for environment adopting patterns similar to dynamic languages. For example type inference (`x := 0` is valid declaration of a variable `x` of type `int`).
*   Compilation time is fast.
*   In built concurrency support: light-weight processes (via goroutines), channels, select statement.
*   Conciseness, Simplicity, and Safety.
*   Support for Interfaces and Type embedding.
*   The go compiler supports static linking. All the go code can be statically linked into one big fat binary and it can be deployed in cloud servers easily without worrying about dependencies.

###### Source

* https://www.tutorialspoint.com/go/go_interview_questions.htm

[[↑] Back to top](#Golang)
### Why the Go language was created?

**Go** was born out of frustration with existing languages and environments for systems programming. 

Go is an attempt to have:
* an interpreted, dynamically typed language with 
* the efficiency and safety of a statically typed, compiled language
* support for networked and multicore computing
* be fast in compilation

To meet these goals required addressing a number of linguistic issues: an expressive but lightweight type system; concurrency and garbage collection; rigid dependency specification; and so on. These cannot be addressed well by libraries or tools so a new language was born.


###### Source

* https://golang.org/doc/faq

[[↑] Back to top](#Golang)
### Does Go have exceptions?

No, Go takes a different approach. For plain error handling, Go's **multi-value returns** make it easy to report an error without overloading the return value. Go code uses error values to indicate an abnormal state. 

Consider:
```go
func Open(name string) (file *File, err error)
```
```go
f, err := os.Open("filename.ext")
if err != nil {
    log.Fatal(err)
}
// do something with the open *File f
```

###### Source

* https://golang.org/doc/faq

[[↑] Back to top](#Golang)
### What are Goroutines?

**Goroutines** are functions or methods that run concurrently with other functions or methods. Goroutines can be thought of as light weight threads. The cost of creating a Goroutine is tiny when compared to a thread. Its common for Go applications to have thousands of Goroutines running concurrently.

###### Source

* https://golangbot.com/goroutines/

[[↑] Back to top](#Golang)
### Let's talk variable declaration in Go. Could you explain what is a variable "zero value"?

Variable is the name given to a memory location to store a value of a specific type. There are various syntaxes to declare variables in go.

```go
// 1 - variable declaration, then assignment
var age int
age = 29

// 2 - variable declaration with initial value
var age2 int = 29

// 3 - Type inference
var age3 = 29

// 4 - declaring multiple variables
var width, height int = 100, 50

// 5 - declare variables belonging to different types in a single statement
var (  
      name1 = initialvalue1,
      name2 = initialvalue2
)
// 6 - short hand declaration
name, age4 := "naveen", 29 //short hand declaration
```

If a variable is not assigned any value, go automatically initialises it with the **zero value of the variable's type**. Go is strongly typed, so variables declared as belonging to one type cannot be assigned a value of another type.

###### Source

* https://golangbot.com/variables/

[[↑] Back to top](#Golang)
### Is Go an object-oriented language?

Yes and no. Although Go has types and methods and allows an object-oriented style of programming, there is no type hierarchy. This is in contrast to most object-oriented languages like C++, Java, C#, Scala, and even dynamic languages like Python and Ruby.

Go Object-Oriented Language Features:
* **Structs** - Structs are user-defined types. Struct types (with methods) serve similar purposes to classes in other languages.
* **Methods** - Methods are functions that operate on particular types. They have a receiver clause that mandates what type they operate on.
* **Embedding** - we can embed anonymous types inside each other. If we embed a nameless struct then the embedded struct provides its state (and methods) to the embedding struct directly.
* **Interfaces** - Interfaces are types that declare sets of methods. Similarly to interfaces in other languages, they have no implementation. Objects that implement all the interface methods automatically implement the interface. There is no inheritance or subclassing or "implements" keyword.

The Go way to implement:
* ** Encapsulation** - Go encapsulates things at the package level. Names that start with a lowercase letter are only visible within that package. You can hide anything in a private package and just expose specific types, interfaces, and factory functions. 
* **Inheritance** - composition by *embedding* an anonymous type is equivalent to implementation inheritance. 
* **Polymorphism** - A variable of type interface can hold any value which implements the interface. This property of interfaces is used to achieve polymorphism in Go.

Consider:
```js
package main

import (  
    "fmt"
)

// interface declaration
type Income interface {  
    calculate() int
    source() string
}

// struct declaration
type FixedBilling struct {  
    projectName string
    biddedAmount int
}

type TimeAndMaterial struct {  
    projectName string
    noOfHours  int
    hourlyRate int
}

// interface implementation for FixedBilling
func (fb FixedBilling) calculate() int {  
    return fb.biddedAmount
}

func (fb FixedBilling) source() string {  
    return fb.projectName
}

// interface implementation for TimeAndMaterial
func (tm TimeAndMaterial) calculate() int {  
    return tm.noOfHours * tm.hourlyRate
}

func (tm TimeAndMaterial) source() string {  
    return tm.projectName
}

// using Polymorphism for calculation based 
// on the array of variables of interface type 
func calculateNetIncome(ic []Income) {  
    var netincome int = 0
    for _, income := range ic {
        fmt.Printf("Income From %s = $%d\n", income.source(), income.calculate())
        netincome += income.calculate()
    }
    fmt.Printf("Net income of organisation = $%d", netincome)
}

func main() {  
    project1 := FixedBilling{projectName: "Project 1", biddedAmount: 5000}
    project2 := FixedBilling{projectName: "Project 2", biddedAmount: 10000}
    project3 := TimeAndMaterial{projectName: "Project 3", noOfHours: 160, hourlyRate: 25}
    incomeStreams := []Income{project1, project2, project3}
    calculateNetIncome(incomeStreams)
}
```

###### Source

* https://golangbot.com/goroutines/

[[↑] Back to top](#Golang)
### Name some advantages of Goroutines over threads

* Goroutines are extremely **cheap to create** when compared to threads. They are only a few kb in stack size and the stack can grow and shrink according to needs of the application whereas in the case of threads the stack size has to be specified and is fixed.
* The Goroutines are **multiplexed** to fewer number of OS threads. There might be only one thread in a program with thousands of Goroutines. If any Goroutine in that thread blocks say waiting for user input, then another OS thread is created and the remaining Goroutines are moved to the new OS thread.
* Goroutines communicate using **channels**. Channels by design **prevent race conditions** (a race condition occurs when two or more threads can access shared data and they try to change it at the same time) from happening when accessing shared memory using Goroutines. Channels can be thought of as a pipe using which Goroutines communicate. 

###### Source

* https://golangbot.com/goroutines/

[[↑] Back to top](#Golang)
### Have you worked with Go 2?

Tricky questions and the answer is no one worked. There is no Go version 2 available in 2018 but there are some movement toward it. Go 1 was released in 2012, and includes a language specification, standard libraries, and custom tools. It provides a stable foundation for creating reliable products, projects, and publications. The purpose of Go 1 is to provide long-term stability. There may well be a Go 2 one day, but not for a few years and it will be influenced by what we learn using Go 1 as it is today.

The possible goals and features of Go 2 are:
* Fix the most significant ways Go fails to scale
*Provide backward compatibility
* Go 2 must not split the Go ecosystem

###### Source

* https://golang.org/doc/faq

[[↑] Back to top](#Golang)
### What is "rune" type in Go?

There are many other symbols invented by humans other than the 'abcde..' symbols. And there are so many that we need 32 bit to encode them. 

A **rune** is a builtin type in Go and it's the alias of `int32`. rune represents a Unicode CodePoint in Go. It does not matter how many bytes the code point occupies, it can be represented by a rune.  For example the rule literal `a` is in reality the number 97.

A string is *not* necessarily a sequence of runes. We can convert between `string` and `[]rune`, but they are different.

###### Source

* https://golangbot.com/types/

[[↑] Back to top](#Golang)
### What is so special about constants in Go?

Constants in Go are special. 

* **Untyped constants.**
Any constant in golang, named or unnamed, is untyped unless given a type explicitly. For example an untyped floating-point constant like `4.5` can be used anywhere a floating-point value is allowed. We can use untyped constants to temporarily escape from Go’s strong type system until their evaluation in a type-demanding expression.
```go
1       // untyped integer constant
const a = 1
var myFloat32 float32 = 4.5
var myComplex64 complex64 = 4.5
```

* **Typed constants**. Constants are typed when you explicitly specify the type in the declaration. With typed constants, you lose all the flexibility that comes with untyped constants like assigning them to any variable of compatible type or mixing them in mathematical operations.
```go
const typedInt int = 1  
```

Generally we should declare a type for a constant only if it’s absolutely necessary. Otherwise, just declare constants without a type.

###### Source

* https://www.callicoder.com/golang-typed-untyped-constants/

[[↑] Back to top](#Golang)
