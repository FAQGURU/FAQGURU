## .NET Framework

[What is the difference between String and string in C#?](#what-is-the-difference-between-string-and-string-in-c)

[What is the .NET Framework?](#what-is-the-net-framework)

[What is .NET Core?](#what-is-net-core)

[What is ASP.NET Core?](#what-is-aspnet-core)

[What is CLR?](#what-is-clr)

[How to configure your ASP.NET Core app?](#how-to-configure-your-aspnet-core-app)

[Talk about Logging in ASP.NET Core?](#talk-about-logging-in-aspnet-core)

[Name some CLR services?](#name-some-clr-services)

[Explain startup process in ASP.NET Core?](#explain-startup-process-in-aspnet-core)

[What is a .NET application domain?](#what-is-a-net-application-domain)

[What is MSIL?](#what-is-msil)

[What is an unmanaged resource? ](#what-is-an-unmanaged-resource-)

[What is Razor Pages?](#what-is-razor-pages)

[What is the difference between .NET Core and Mono?](#what-is-the-difference-between-net-core-and-mono)

[Can ASP.NET Core work with the .NET framework?](#can-aspnet-core-work-with-the-net-framework)

[What are some characteristics of .NET Core?](#what-are-some-characteristics-of-net-core)

[What is the difference between decimal, float and double in .NET? ](#what-is-the-difference-between-decimal-float-and-double-in-net-)

[What's the difference between SDK and Runtime in .NET Core?](#whats-the-difference-between-sdk-and-runtime-in-net-core)

[What is CTS?](#what-is-cts)

[What is .NET Standard?](#what-is-net-standard)

[Explain the difference between “managed” and “unmanaged” code?](#explain-the-difference-between-managed-and-unmanaged-code)

[Explain two types of deployment for .NET Core applications](#explain-two-types-of-deployment-for-net-core-applications)

[What is Kestrel?](#what-is-kestrel)

[What is CoreCLR?](#what-is-coreclr)

[Explain usage of Dependency Injection in ASP.NET Core](#explain-usage-of-dependency-injection-in-aspnet-core)

[Explain what is included in .NET Core?](#explain-what-is-included-in-net-core)

[What is difference between .NET Core and .NET Framework?](#what-is-difference-between-net-core-and-net-framework)

[Is there a way to catch multiple exceptions at once and without code duplication?](#is-there-a-way-to-catch-multiple-exceptions-at-once-and-without-code-duplication)

[What is new in ASP.NET Core 2, compared to ASP.NET Core 1?](#what-is-new-in-aspnet-core-2-compared-to-aspnet-core-1)

[Why to use of the IDisposable interface?](#why-to-use-of-the-idisposable-interface)

[Explain Middleware in ASP.NET Core?](#explain-middleware-in-aspnet-core)

[What does Common Language Specification (CLS) mean?](#what-does-common-language-specification-cls-mean)

[Talk about new .csproj file?](#talk-about-new-csproj-file)

[Explain the difference between Task and Thread in .NET](#explain-the-difference-between-task-and-thread-in-net)

[What is FCL?](#what-is-fcl)

[What's the difference between .NET Core, .NET Framework, and Xamarin?](#whats-the-difference-between-net-core-net-framework-and-xamarin)

[What is implicit compilation?](#what-is-implicit-compilation)

[What is JIT compiler?](#what-is-jit-compiler)

[What about NuGet packages and packages.config?](#what-about-nuget-packages-and-packagesconfig)

[What is Explicit Compilation?](#what-is-explicit-compilation)

[What are the benefits of explicit compilation?](#what-are-the-benefits-of-explicit-compilation)

[What's is BCL?](#whats-is-bcl)

[Why does .NET use a JIT compiler instead of just compiling the code once on the target machine?](#why-does-net-use-a-jit-compiler-instead-of-just-compiling-the-code-once-on-the-target-machine)

[What are benefits of using JIT?](#what-are-benefits-of-using-jit)

[What is the difference between AppDomain, Assembly, Process, and a Thread?](#what-is-the-difference-between-appdomain-assembly-process-and-a-thread)

[Explain how does Asynchronous tasks (Async/Await) work in .NET?](#explain-how-does-asynchronous-tasks-asyncawait-work-in-net)

[What is the difference between CIL and MSIL (IL)?](#what-is-the-difference-between-cil-and-msil-il)

[What is the difference between .NET Framework/Core and .NET Standard Class Library project types?](#what-is-the-difference-between-net-frameworkcore-and-net-standard-class-library-project-types)

[What's the difference between RyuJIT and Roslyn?](#whats-the-difference-between-ryujit-and-roslyn)

[What is the difference between ASP.NET Core Web (.NET Core) vs ASP.NET Core Web (.NET Framework)?](#what-is-the-difference-between-aspnet-core-web-net-core-vs-aspnet-core-web-net-framework)

[How many types of JIT Compilations do you know?](#how-many-types-of-jit-compilations-do-you-know)

[What is the difference between Node.js async model and async/await in .NET?](#what-is-the-difference-between-nodejs-async-model-and-asyncawait-in-net)

[Explain Finalize vs Dispose usage?](#explain-finalize-vs-dispose-usage)



### What is the difference between String and string in C#?

`string` is an alias in C# for `System.String`. So technically, there is no difference. It's like `int` vs. `System.Int32`.

As far as guidelines, it's generally recommended to use `string` any time you're referring to an object.
```csharp
string place = "world";
```

Likewise, it's generally recommended to use `String` if you need to refer specifically to the class.
```csharp
string greet = String.Format("Hello {0}!", place);
```

###### Source

* https://stackoverflow.com/questions/618535/difference-between-decimal-float-and-double-in-net

[[↑] Back to top](#net-framework)
### What is the .NET Framework?

The .NET is a Framework, which is a collection of classes of reusable libraries given by Microsoft to be used in other .NET applications and to develop, build and deploy many types of applications on the Windows platform including the following:

*   Console Applications
*   Windows Forms Applications
*   Windows Presentation Foundation (WPF) Applications
*   Web Applications
*   Web Services
*   Windows Services
*   Services-oriented applications using Windows Communications Foundation (WCF)
*   Workflow-enabled applications using Windows Workflow Foundation(WF)

###### Source

* https://www.c-sharpcorner.com/UploadFile/8ef97c/interview-question-on-net-framework-or-clr/

[[↑] Back to top](#net-framework)
### What is .NET Core?

The .NET Core platform is a new .NET stack that is optimized for open source development and agile delivery on NuGet. 

.NET Core has two major components. It includes a small runtime that is built from the same codebase as the .NET Framework CLR. The .NET Core runtime includes the same GC and JIT (RyuJIT), but doesn’t include features like Application Domains or Code Access Security. The runtime is delivered via NuGet, as part of the ASP.NET Core package.

.NET Core also includes the base class libraries. These libraries are largely the same code as the .NET Framework class libraries, but have been factored (removal of dependencies) to enable to ship a smaller set of libraries. These libraries are shipped as `System.*` NuGet packages on NuGet.org.

###### Source

* https://stackoverflow.com/questions/26908049/what-is-net-core

[[↑] Back to top](#net-framework)
### What is ASP.NET Core?

ASP.NET Core is a brand new cross-platform web framework built with .NET Core framework. It is not an update to existing ASP.NET framework. It is a complete rewrite of the ASP.NET framework. It works with both .NET Core and .NET Framework.

Main characterestics of ASP.NET Core:

*   DI Container which is quite simple and built-in. You can extend it with other popular DI containers
*   Built-in and extensible structured logging. You can redirect output to as many sources as you want (file, Azure, AWS, console)
*   Extensible strongly typed configuration, which can also be used to reload at run-time
*   Kestrel – new, cross-platform and super fast web server which can stand alone without IIS, Nginx or Apache
*   New, fully async pipeline. It is easily configured via middleware
*   ASP.NET All meta package which improves development speed, and enables you to reference all Microsoft packages for ASP.NET Core and it will deploy only those that are being used by your code
*   There is no _web.config_. We now use _appsettings.json_ file in combination with other sources of configuration (command line args, environment variables, etc.)
*   There is no _Global._asax – We have _Startup.cs_ which is used to set up Middleware and services for DI Container.

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### What is CLR?

The **CLR** stands for Common Language Runtime and it is an Execution Environment. It works as a layer between Operating Systems and the applications written in .NET languages that conforms to the Common Language Specification (CLS). The main function of Common Language Runtime (CLR) is to convert the Managed Code into native code and then execute the program.

###### Source

* https://www.c-sharpcorner.com/UploadFile/8ef97c/interview-question-on-net-framework-or-clr/

[[↑] Back to top](#net-framework)
### How to configure your ASP.NET Core app?

Another crucial part of ASP.NET Core Framework is Configuration. Also, it is part of Dependency Injection. Use it anywhere in your code with an option to [reload on changes](https://codingblast.com/asp-net-core-configuration-reloading-binding-injecting/) of configuration values from sources (appsettings.json, environment variables, command line arguments, etc.). It is also easy to override, extend and customize the Configuration. No more extensive configurations in web.config, the preferred way now is _**appsettings.json**_ in combination with a mix of Environment variables and cmd-line args.

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### Talk about Logging in ASP.NET Core?

**Logging** is built-in and you get access to structured logs from the ASP.NET Core host itself to your application. With tools like [Serilog,](https://github.com/serilog/serilog-aspnetcore) you can extend your logging [easily](https://github.com/serilog/serilog-sinks-rollingfile) and save your logs to file, Azure, Amazon or any other output provider. You can configure verbosity and log levels via configuration (appsettings.json by default), and you can configure log levels by different categories.

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### Name some CLR services?

**CLR services**

*   Assembly Resolver
*   Assembly Loader
*   Type Checker
*   COM marshalled
*   Debug Manager
*   Thread Support
*   IL to Native compiler
*   Exception Manager
*   Garbage Collector

###### Source

* https://www.c-sharpcorner.com/UploadFile/8ef97c/interview-question-on-net-framework-or-clr/

[[↑] Back to top](#net-framework)
### Explain startup process in ASP.NET Core?

Everything starts from Program.cs
```csharp
public static void Main(string[] args)
{
    BuildWebHost(args).Run();
}
 
public static IWebHost BuildWebHost(string[] args) =>
    WebHost.CreateDefaultBuilder(args)
        .UseStartup<Startup>()
        .Build();
```

CreateDefaultBuilder extension method will create a default configuration which will look first into `appsettings.json` files then will look for Environment variables and at the end, it will use command line arguments.

This part will also set up default logger sources (debug and console) and load the settings for logging from appsettings.json.

After the `CreateDefaultBuilder` finishes, then `Startup` class is executed. First, the constructor code is executed. After that, services are added to DI container via `AddServices` method that lives in Startup class. After that, an order of middleware that will handle every incoming request is set up.

###### Source

* https://codingblast.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### What is a .NET application domain?

It is an isolation layer provided by the .NET runtime. As such, App domains live with in a process (1 process can have many app domains) and have their own virtual address space.

App domains are useful because:

* They are less expensive than full processes
* They are multithreaded
* You can stop one without killing everything in the process
* Segregation of resources/config/etc
* Each app domain runs on its own security level

###### Source

* https://stackoverflow.com/questions/1094478/what-is-a-net-application-domain

[[↑] Back to top](#net-framework)
### What is MSIL?

When we compile our .NET code then it is not directly converted to native/binary code; it is first converted into intermediate code known as MSIL code which is then interpreted by the CLR. MSIL is independent of hardware and the operating system. Cross language relationships are possible since MSIL is the same for all .NET languages. MSIL is further converted into native code.  

###### Source

* https://www.c-sharpcorner.com/UploadFile/8ef97c/interview-question-on-net-framework-or-clr/

[[↑] Back to top](#net-framework)
### What is an unmanaged resource? 

Use that rule of thumb: 
* If you found it in the Microsoft .NET Framework: _it's managed_. 
* If you went poking around MSDN yourself, _it's unmanaged_. 

Anything you've used P/Invoke calls to get outside of the nice comfy world of everything available to you in the .NET Framwork is unmanaged – and you're now _responsible_ for cleaning it up.

###### Source

* https://stackoverflow.com/questions/538060/proper-use-of-the-idisposable-interface

[[↑] Back to top](#net-framework)
### What is Razor Pages?

[Razor Pages](https://codingblast.com/asp-net-core-razor-pages/) is a new feature of ASP.NET Core that makes coding page-focused scenarios easier and more productive.

With Razor Pages, you have this one Razor file (_.cshtml_), and the code for a single page lives inside of that file, and that file also represents the URL structure of the app. Therefore, you got everything inside of one file, and it just works.

However, you can separate your code to the _code behind_ file with _.cshtml.cs_ extension. You would usually have your view model and handlers (like action methods in MVC) in that file and handle the logic there. Of course, you could also have your view model moved to separate place.

Since Razor Pages is part of the MVC stack, you can use anything that comes with MVC inside of our Razor Pages.

###### Source

* https://codingblast.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### What is the difference between .NET Core and Mono?

To be simple:
* Mono is third party implementation of .Net Framework for Linux/Android/iOs
* .Net Core is Microsoft's own implementation for same.

###### Source

* https://stackoverflow.com/questions/37738106/net-core-vs-mono

[[↑] Back to top](#net-framework)
### Can ASP.NET Core work with the .NET framework?

Yes. This might surprise many, but ASP.NET Core works with .NET framework and this is officially supported by Microsoft.

ASP.NET Core works with:

*   .NET Core framework
*   .NET framework

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### What are some characteristics of .NET Core?

* **Flexible deployment**: Can be included in your app or installed side-by-side user- or machine-wide.

* **Cross-platform**: Runs on Windows, macOS and Linux; can be ported to other OSes. The supported Operating Systems (OS), CPUs and application scenarios will grow over time, provided by Microsoft, other companies, and individuals.

* **Command-line tools**: All product scenarios can be exercised at the command-line.

* **Compatible**: .NET Core is compatible with .NET Framework, Xamarin and Mono, via the .NET Standard Library.

* **Open source**: The .NET Core platform is open source, using MIT and Apache 2 licenses. Documentation is licensed under CC-BY. .NET Core is a .NET Foundation project.

* **Supported by Microsoft**: .NET Core is supported by Microsoft, per .NET Core Support

###### Source

* https://stackoverflow.com/questions/26908049/what-is-net-core

[[↑] Back to top](#net-framework)
### What is the difference between decimal, float and double in .NET? 

Precision is the main difference.

* Float - 7 digits (32 bit)
* Double-15-16 digits (64 bit)
* Decimal -28-29 significant digits (128 bit)

As for what to use when:

* For values which are "naturally exact decimals" it's good to use decimal. This is usually suitable for any concepts invented by humans: financial values are the most obvious example, but there are others too. Consider the score given to divers or ice skaters, for example.

* For values which are more artefacts of nature which can't really be measured exactly anyway, float/double are more appropriate. For example, scientific data would usually be represented in this form. Here, the original values won't be "decimally accurate" to start with, so it's not important for the expected results to maintain the "decimal accuracy". Floating binary point types are much faster to work with than decimals.

###### Source

* https://stackoverflow.com/questions/618535/difference-between-decimal-float-and-double-in-net

[[↑] Back to top](#net-framework)
### What's the difference between SDK and Runtime in .NET Core?

* The SDK is all of the stuff that is needed/makes developing a .NET Core application easier, such as the CLI and a compiler.

* The runtime is the "virtual machine" that hosts/runs the application and abstracts all the interaction with the base operating system.

###### Source

* https://stackoverflow.com/questions/47733014/whats-the-difference-between-sdk-and-runtime-in-net-core

[[↑] Back to top](#net-framework)
### What is CTS?

The **Common Type System (CTS)** standardizes the data types of all programming languages using .NET under the umbrella of .NET to a common data type for easy and smooth communication among these .NET languages. 

CTS is designed as a singly rooted object hierarchy with `System.Object` as the base type from which all other types are derived. CTS supports two different kinds of types: 

1. **Value Types**: Contain the values that need to be stored directly on the stack or allocated inline in a structure. They can be built-in (standard primitive types), user-defined (defined in source code) or enumerations (sets of enumerated values that are represented by labels but stored as a numeric type).
2. **Reference Types**: Store a reference to the value‘s memory address and are allocated on the heap. Reference types can be any of the pointer types, interface types or self-describing types (arrays and class types such as user-defined classes, boxed value types and delegates).

###### Source

* https://www.c-sharpcorner.com/UploadFile/8ef97c/interview-question-on-net-framework-or-clr/

[[↑] Back to top](#net-framework)
### What is .NET Standard?

* .NET Standard solves the code sharing problem for .NET developers across all platforms by bringing all the APIs that you expect and love across the environments that you need: desktop applications, mobile apps & games, and cloud services
* .NET Standard is a set of APIs that all .NET platforms have to implement. This unifies the .NET platforms and prevents future fragmentation.
* .NET Standard 2.0 will be implemented by .NET Framework, .NET Core, and Xamarin. For .NET Core, this will add many of the existing APIs that have been requested.
* .NET Standard 2.0 includes a compatibility shim for .NET Framework binaries, significantly increasing the set of libraries that you can reference from your .NET Standard libraries.
* .NET Standard will replace Portable Class Libraries (PCLs) as the tooling story for building multi-platform .NET libraries.

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### Explain the difference between “managed” and “unmanaged” code?

* **Managed** code is not compiled to machine code but to an intermediate language which is interpreted and executed by some service on a machine and is therefore operating within a (hopefully!) secure framework which handles dangerous things like memory and threads for you. It runs on the CLR (Common Language Runtime), which, among other things, offers services like garbage collection, run-time type checking, and reference checking. So, think of it as, "My code is _managed_ by the CLR."

* **Unmanaged code** is compiled to machine code and therefore executed by the OS directly. It therefore has the ability to do damaging/powerful things Managed code does not. This is how everything used to work, so typically it's associated with old stuff like .dlls

###### Source

* https://stackoverflow.com/questions/3563870/difference-between-managed-and-unmanaged

[[↑] Back to top](#net-framework)
### Explain two types of deployment for .NET Core applications

* **Framework-dependent deployment (FDD)** - it relies on the presence of a shared system-wide version of .NET Core on the target system. The app contains only its own code and any third-party dependencies that are outside of the .NET Core libraries. FDDs contain .dll files that can be launched by using the dotnet utility from the command line. 

 ```sh
dotnet app.dll
```
* **Self-contained deployment** - Unlike FDD, a self-contained deployment (SCD) doesn't rely on the presence of shared components on the target system. All components, including both the .NET Core libraries and the .NET Core runtime, are included with the application and are isolated from other .NET Core applications. SCDs include an executable (such as app.exe on Windows platforms for an application named app), which is a renamed version of the platform-specific .NET Core host, and a .dll file (such as app.dll), which is the actual application.

###### Source

* https://docs.microsoft.com/en-us/dotnet/core/deploying/index

[[↑] Back to top](#net-framework)
### What is Kestrel?

*   Kestrel is a cross-platform web server built for ASP.NET Core based on libuv – a cross-platform asynchronous I/O library.
*   It is a default web server pick since it is used in all ASP.NET Core templates.
*   It is really fast.
*   It is secure and good enough to use it without a reverse proxy server. However, it is still recommended that you use IIS, Nginx or Apache or something else.

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### What is CoreCLR?

CoreCLR is the .NET execution engine in .NET Core, performing functions such as garbage collection and compilation to machine code. 

Consider:
<div class="text-center">
<img src="https://i.stack.imgur.com/nWPth.png" class="img-fluid"/>
</div>

###### Source

* https://blogs.msdn.microsoft.com/dotnet/2015/02/03/coreclr-is-now-open-source/

[[↑] Back to top](#net-framework)
### Explain usage of Dependency Injection in ASP.NET Core

**Dependency Injection **comes as a part of ASP.NET Core Framework and everything is built around it. When you want to use some tool and its services, you usually add the NuGet package and you use one of its extension methods to add the package to the ASP.NET Core’s DI container. You can extend the current DI with a container of your choice (AutoFac, StructureMap, CastleWindsor etc).

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### Explain what is included in .NET Core?

* A .NET runtime, which provides a type system, assembly loading, a garbage collector, native interop and other basic services.

* A set of framework libraries, which provide primitive data types, app composition types and fundamental utilities.

* A set of SDK tools and language compilers that enable the base developer experience, available in the .NET Core SDK.

* The 'dotnet' app host, which is used to launch .NET Core apps. It selects the runtime and hosts the runtime, provides an assembly loading policy and launches the app. The same host is also used to launch SDK tools in much the same way.

###### Source

* https://stackoverflow.com/questions/26908049/what-is-net-core

[[↑] Back to top](#net-framework)
### What is difference between .NET Core and .NET Framework?

.NET as whole now has 2 flavors:

* .NET Framework
* .NET Core

*.NET Core* and the *.NET Framework* have (for the most part) a subset-superset relationship. .NET Core is named “Core” since it contains the core features from the .NET Framework, for both the runtime and framework libraries. For example, .NET Core and the .NET Framework share the GC, the JIT and types such as `String` and `List`.

.NET Core was created so that .NET could be open source, cross platform and be used in more resource-constrained environments.

###### Source

* https://stackoverflow.com/questions/10448516/apache-jmeter-listener-results-interpretation

[[↑] Back to top](#net-framework)
### Is there a way to catch multiple exceptions at once and without code duplication?

Catch System.Exception and switch on the types:
```csharp
catch (Exception ex)            
{                
    if (ex is FormatException || ex is OverflowException)
    {
        WebId = Guid.Empty;
        return;
    }

    throw;
}
```

###### Source

* https://stackoverflow.com/questions/125319/should-using-directives-be-inside-or-outside-the-namespace

[[↑] Back to top](#net-framework)
### What is new in ASP.NET Core 2, compared to ASP.NET Core 1?

With ASP.NET Core 2 several new features came out:

*   Razor Pages
*   DbContext Pooling with Entity Framework Core 2
*   Simplified Application Host Configuration
*   Configuration is now part of DI and ready for the time server reaches _Startup_ class
*   Simplified authentication model
*   **_dotnet new_** now restore NuGet packages automatically
*   New meta package – _**Microsoft.AspNetCore.All**_

###### Source

* https://codingblast.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### Why to use of the IDisposable interface?

The "primary" use of the `IDisposable` interface is to clean up unmanaged resources. Note the purpose of the Dispose pattern is to provide a mechanism to clean up both _managed_ and _unmanaged_ resources and when that occurs depends on how the Dispose method is being called. 

###### Source

* https://stackoverflow.com/questions/538060/proper-use-of-the-idisposable-interface

[[↑] Back to top](#net-framework)
### Explain Middleware in ASP.NET Core?

Middleware is actually sequential series of delegates (piece of code), that can either short-circuit or pass on the HTTP request to next delegate. These are known as middleware, a concept well known to people who worked with Node.js.

Piece of your middleware can do one of the following:

*   Handle an incoming HTTP request by generating an HTTP response (maybe your authentication or authorization middleware will stop the request early and immediately create response)
*   Process the incoming request, change it and pass it to the next middleware in the pipeline
*   Process the outgoing response, change it and pass it on to next middleware in the pipeline or directly to the ASP.NET Core web server

###### Source

* http://www.talkingdotnet.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### What does Common Language Specification (CLS) mean?

The **Common Language Specification (CLS)** is a fundamental set of language features supported by the Common Language Runtime (CLR) of the .NET Framework. CLS is a part of the specifications of the .NET Framework. CLS was designed to support language constructs commonly used by developers and to produce verifiable code, which allows all CLS-compliant languages to ensure the type safety of code. CLS includes features common to many object-oriented programming languages. It forms a subset of the functionality of common type system (CTS) and has more rules than defined in CTS.

###### Source

* https://www.techopedia.com/definition/25318/common-language-specification-cls-net

[[↑] Back to top](#net-framework)
### Talk about new .csproj file?

_**.csproj**_ file is now used as a place where we manage the NuGet packages for your application.

File explorer and project explorer are now in sync. For .NET Core projects, you can easily drop a file from file explorer into a project or delete it from the file system and it will be gone from the project. No more source files in** a .csproj** file.

You can now edit the **.csproj** file directly without unloading the project.


###### Source

* https://codingblast.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### Explain the difference between Task and Thread in .NET

* **Thread** represents an actual OS-level thread, with its own stack and kernel resources.  Thread allows the highest degree of control; you can Abort() or Suspend() or Resume() a thread, you can observe its state, and you can set thread-level properties like the stack size, apartment state, or culture. ThreadPool is a wrapper around a pool of threads maintained by the CLR.

* The **Task class** from the Task Parallel Library offers the best of both worlds. Like the ThreadPool, a task does not create its own OS thread. Instead, tasks are executed by a TaskScheduler; the default scheduler simply runs on the ThreadPool. Unlike the ThreadPool, Task also allows you to find out when it finishes, and (via the generic Task) to return a result. 

###### Source

* https://stackoverflow.com/questions/13429129/task-vs-thread-differences

[[↑] Back to top](#net-framework)
### What is FCL?

The .NET Framework class library is exactly what its name suggests: a library of classes and other types that developers can use to make their lives easier. While these classes are themselves written in C#, they can be used from any CLR based language.

The **Framework Class Library (FCL)** is the wider library that contains the totality: ASP.NET, WinForms, the XML stack, ADO.NET and more. You could say that the FCL includes the BCL.

On a simple level, .NET Framework = libraries (FCL, BCL), language compilers (C#, VB.NET) and Common Language Runtime (CLR).

###### Source

* https://stackoverflow.com/questions/807880/bcl-base-class-library-vs-fcl-framework-class-library

[[↑] Back to top](#net-framework)
### What's the difference between .NET Core, .NET Framework, and Xamarin?

* **.NET Framework** is the "full" or "traditional" flavor of .NET that's distributed with Windows. Use this when you are building a desktop Windows or UWP app, or working with older ASP.NET 4.6+.
* **.NET Core** is cross-platform .NET that runs on Windows, Mac, and Linux. Use this when you want to build console or web apps that can run on any platform, including inside Docker containers. This does not include UWP/desktop apps currently.
* **Xamarin** is used for building mobile apps that can run on iOS, Android, or Windows Phone devices.

<img src="https://i.stack.imgur.com/CtALu.jpg" class="img-fluid"/>

Xamarin usually runs on top of Mono, which is a version of .NET that was built for cross-platform support before Microsoft decided to officially go cross-platform with .NET Core. Like Xamarin, the Unity platform also runs on top of Mono.

###### Source

* https://stackoverflow.com/questions/38063837/whats-the-difference-between-net-core-net-framework-and-xamarin

[[↑] Back to top](#net-framework)
### What is implicit compilation?

**Implicit Compilation** is a two-steps process, and it requires a Virtual Machine to be able to execute your code. 

* The first step of the process is converting your program to a bytecode understandable by Virtual Machine. .NET bytecode is called Common Intermediate Language or CIL. It is also known as Microsoft Intermediate Language (MSIL) or just Intermediate Language (IL).
* The second step is converting CIL code to a machine code running on metal. This is Virtual Machine’s task. Common Language Runtime (.NET Virtual Machine) converts only executed CIL fragments into CPU instructions at runtime. The .NET framework calls this compiler the JIT (Just-In-Time) compiler. 

###### Source

* http://geekswithblogs.net/ilich/archive/2013/07/09/.net-compilation-part-1.-just-in-time-compiler.aspx

[[↑] Back to top](#net-framework)
### What is JIT compiler?

Before a computer can execute the source code, special programs called compilers must rewrite it into machine instructions, also known as object code. This process (commonly referred to simply as “compilation”) can be done explicitly or implicitly.

Implicit compilation is a two-step process:
* The first step is converting the source code to intermediate language (IL) by a language-specific compiler. 
* The second step is converting the IL to machine instructions. The main difference with the explicit compilers is that only executed fragments of IL code are compiled into machine instructions, at runtime. The .NET framework calls this compiler the **JIT (Just-In-Time) compiler**.

###### Source

* https://www.telerik.com/blogs/understanding-net-just-in-time-compilation

[[↑] Back to top](#net-framework)
### What about NuGet packages and packages.config?

There is no more _packages.config_ file. All packages are now managed within _.csproj_ file.

The **.csproj** file has been cleaned up and it also serves the role of packages.config(or package.json for Node devs). That means that’s where your packages and versions will be saved.

NuGet packages are the unit of reference and they can depend on other NuGet packages, but also they can depend on projects. And as before, projects can also depend on NuGet packages and other projects. That means that projects and NuGet packages are interchangeable.

With .NET Core, you can easily turn your projects into NuGet packages, with one click inside of the properties.

###### Source

* https://codingblast.com/asp-net-core-interview-questions/

[[↑] Back to top](#net-framework)
### What is Explicit Compilation?

**Explicit compilation** converts the upper level language into object code prior to program execution. Ahead of time (AOT) compilers are designed to ensure that, the CPU can understand every line in the code before any interaction takes place.

###### Source

* https://www.telerik.com/blogs/understanding-net-just-in-time-compilation

[[↑] Back to top](#net-framework)
### What are the benefits of explicit compilation?

**Ahead of time (AOT)** delivers faster start-up time, especially in large applications where much code executes on startup. But it requires more disk space and more memory/virtual address space to keep both the IL and precompiled images. In this case the JIT Compiler has to do a lot of disk I/O actions, which are quite expensive.

###### Source

* https://www.telerik.com/blogs/understanding-net-just-in-time-compilation

[[↑] Back to top](#net-framework)
### What's is BCL?

A .NET Framework library, BCL is the standard for the C# runtime library and one of the Common Language Infrastructure (CLI) standard libraries. BCL provides types representing the built-in CLI data types, basic file access, collections, custom attributes, formatting, security attributes, I/O streams, string manipulation, and more.

The Base Class Library (BCL) is literally that, the base. It contains basic, fundamental types like System.String and System.DateTime.

###### Source

* https://stackoverflow.com/questions/807880/bcl-base-class-library-vs-fcl-framework-class-library

[[↑] Back to top](#net-framework)
### Why does .NET use a JIT compiler instead of just compiling the code once on the target machine?

There are two things to be gained by using an intermediate format like .NET or Java:

1. You can run the program on any platform, exactly because the code is represented in an intermediate format instead of native code. You just need to write an interpreter for the intermediate format.
2. It allows for some run-time optimizations which are not (easily) possible at compile-time: for example, you can take advantage of special features on new CPUs, even if those CPUs didn't exist when you wrote your program - only the JIT compiler needs to know about that.

###### Source

* https://stackoverflow.com/questions/3842664/why-does-net-use-a-jit-compiler-instead-of-just-compiling-the-code-once-on-the

[[↑] Back to top](#net-framework)
### What are benefits of using JIT?

* JIT can generate faster code, because it targets the current platform of execution. AOT compilation must target the lowest common denominator among all possible execution platforms.
* JIT can profile the application while it runs, and dynamically re-compile the code to deliver better performance in the hot path (the most used functions).

###### Source

* https://www.telerik.com/blogs/understanding-net-just-in-time-compilation

[[↑] Back to top](#net-framework)
### What is the difference between AppDomain, Assembly, Process, and a Thread?

* An **AppDomain** is an isolation unit within a process.  AppDomains can be created at runtime, loaded with code, and unloaded.  Its an isolation boundary designed to make .NET apps more reliable.  
* An **assembly** holds one or more modules, which hold compiled chunks of code.  You will typically see an assembly as an .EXE or a .DLL.
* A **process** is an executing application (waaaay oversimplified).
* A **thread** is an execution context. The operating system executes code within a thread.  The operating system switches between threads, allowing each to execute in turn, thus giving the impression that multiple applications are running at the same time.

To put it all together (very simplified)...

A program is executed.  A process is created by the operating system, and within its single thread it starts loading code to execute.  In a .NET application, a single AppDomain is created by the CLR.  The application's executing assembly (the .EXE) is loaded into this AppDomain and begins execution.  The application can spawn new processes, create AppDomains, load other assemblies into these domains, and then create new Threads to execute code in any of these AppDomains.

###### Source

* https://stackoverflow.com/questions/733868/difference-between-appdomain-assembly-process-and-a-thread/733902#733902

[[↑] Back to top](#net-framework)
### Explain how does Asynchronous tasks (Async/Await) work in .NET?

`await` pauses _the method_ until the operation completes. So the second `await` would get executed after the first `await` returns. 

The purpose of `await` is that it will return the current thread to the thread pool while the awaited operation runs off and does whatever. 

This is particularly useful in high-performance environments, say a web server, where a given request is processed on a given thread from the overall thread pool. If we don't await, then the given thread processing the request (and all it's resources) remains "in use" while the db / service call completes. This might take a couple of seconds or more especially for external service calls.

###### Source

* https://stackoverflow.com/questions/13082074/brief-explanation-of-async-await-in-net-4-5

[[↑] Back to top](#net-framework)
### What is the difference between CIL and MSIL (IL)?

CIL is the term used in the CLI Standard. MSIL is (I suppose) CIL created by MS tools. Effectively they are synonymous.

* CIL – Common Intermediate Language – is the term used in the International Standard.
* MSIL – Microsoft Intermediate Language – is the product term for the Microsoft implementation of that standard.

###### Source

* https://stackoverflow.com/questions/293800/what-is-the-difference-between-cil-and-msil-il/293801

[[↑] Back to top](#net-framework)
### What is the difference between .NET Framework/Core and .NET Standard Class Library project types?

Use a .NET Standard library when you want to increase the number of apps that will be compatible with your library, and you are okay with a decrease in the .NET API surface area your library can access.

Implementing a .Net Standard Library allows code sharing across all different flavours of .NET applications like .NET Framework, .NET Core and Xamarin.


###### Source

* https://stackoverflow.com/questions/42939454/what-is-the-difference-between-net-core-and-net-standard-class-library-project

[[↑] Back to top](#net-framework)
### What's the difference between RyuJIT and Roslyn?

* **Roslyn** is the compiler that compile your code (C# or VB) to IL.
* **RyuJIT** is a Just In Time compiler that compile your IL to a native code.

Both of them are now open source.

###### Source

* https://stackoverflow.com/questions/38340565/whats-the-difference-between-ryujit-and-roslyn

[[↑] Back to top](#net-framework)
### What is the difference between ASP.NET Core Web (.NET Core) vs ASP.NET Core Web (.NET Framework)?

* **ASP.NET Core on .NET Core** is cross-platform ASP.NET Core. It can run on Windows, Mac, and Linux (including Docker). The server doesn't need .NET Core installed - the dependencies can be bundled with the application.

 ASP.NET Core ships entirely as NuGet packages. This allows you to optimize your app to include only the necessary NuGet packages. In fact, ASP.NET Core 2.x apps targeting .NET Core only require a single NuGet package. The benefits of a smaller app surface area include tighter security, reduced servicing, and improved performance.

 It is not required to install .Net framework to run asp.net core with .net core application. An ASP.NET Core application with .net core is a console app that creates a web server in its Main method. It uses Kestrel web server to run the application.

* **ASP.NET Core on .NET Framework** is ASP.NET Core on the "full" or "desktop" .NET Framework (e.g. .NET Framework 4.6.2). These applications can only run on Windows, but everything else about ASP.NET Core behaves the same way. It also supports Aspx, WPF, WCF and WebServices.

###### Source

* https://stackoverflow.com/questions/37684508/difference-between-asp-net-core-net-core-and-asp-net-core-net-framework

[[↑] Back to top](#net-framework)
### How many types of JIT Compilations do you know?

There are **three types** of JIT compilation in the .NET framework:
1. **Pre-JIT** complies complete source code into native code in a single compilation cycle. In .NET languages, this is implemented in Ngen.exe (Native Image Generator). All CIL instructions are compiled to native code before startup. This way the runtime can use native images from the cache instead of invoking the JIT Compiler.
2. **Econo-JIT** complies only those methods that are called at runtime. However, these complied methods are removed when they are not required. 
3. **Normal-JIT** complies only those methods that are called at runtime. These methods are complied the first time they are called, and then they are stored in cache. When the same methods are called again, the complied code from cache is used for execution. 

###### Source

* https://www.c-sharpcorner.com/interview-question/how-many-types-of-jit-compilers

[[↑] Back to top](#net-framework)
### What is the difference between Node.js async model and async/await in .NET?

The async model that has Node.js is similar to the old async model in C# and .Net called Event-based Asynchronous Pattern (EAP). The C#'s async/await keywords make asynchronous code linear and let you avoid "Callback Hell" much better then in any of other programming languages. 

Node.js is asynchronously _single-threaded_, while ASP.NET is asynchronously _multi-threaded_. This means the Node.js code can make some simplifying assumptions because all your code always runs on the same exact thread. So when your ASP.NET code _awaits_, it could possibly resume on a different thread, and it's up to you to avoid things like thread-local state.

The same difference is also a strength for ASP.NET, because it means async ASP.NET can scale out-of-the-box up to the full capabilities of your sever. If you consider, say, an 8-core machine, then ASP.NET can process (the synchronous portions of) 8 requests simultaneously. If you put Node.js on a souped-up server, then it's common to actually run 8 separate instances of Node.js and add something like nginx or a simple custom load balancer that handles routing requests for that server. 


###### Source

* https://stackoverflow.com/questions/21336976/node-js-vs-async-await-in-net

[[↑] Back to top](#net-framework)
### Explain Finalize vs Dispose usage?

* The **finalizer method** is called when your object is garbage collected and you have no guarantee when this will happen (you can force it, but it will hurt performance).

* The **Dispose method**, on the other hand, is meant to be called by the code that created your class so that you can clean up and release any resources you have acquired (unmanaged data, database connections, file handles, etc) the moment the code is done with your object.

The standard practice is to implement `IDisposable` and `Dispose` so that you can use your object in a `using` statement such as `using(var foo = new MyObject()) { }`. And in your finalizer, you call `Dispose`, just in case the calling code forgot to dispose of you.

###### Source

* https://stackoverflow.com/questions/732864/finalize-vs-dispose

[[↑] Back to top](#net-framework)
