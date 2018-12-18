## ASP.NET

[What is ViewData?](#what-is-viewdata)

[What is ASP.Net?](#what-is-aspnet)

[What is ViewState?](#what-is-viewstate)

[How you can add an event handler?](#how-you-can-add-an-event-handler)

[What's the use of Response.Output.Write()?](#whats-the-use-of-responseoutputwrite)

[What is the difference between ASP.NET and ASP.NET MVC?](#what-is-the-difference-between-aspnet-and-aspnet-mvc)

[What is a postback?](#what-is-a-postback)

[What is the good practice to implement validations in aspx page?](#what-is-the-good-practice-to-implement-validations-in-aspx-page)

[What is the file extension of ASP.NET web service?](#what-is-the-file-extension-of-aspnet-web-service)

[What is the meaning of Unobtrusive JavaScript?](#what-is-the-meaning-of-unobtrusive-javascript)

[Explain JSON Binding?](#explain-json-binding)

[What are the different types of caching?](#what-are-the-different-types-of-caching)

[What are the sub types of ActionResult?](#what-are-the-sub-types-of-actionresult)

[ How do you register JavaScript for webcontrols?](#-how-do-you-register-javascript-for-webcontrols)

[What is the difference between Server.Transfer and Response.Redirect?](#what-is-the-difference-between-servertransfer-and-responseredirect)

[Where the viewstate is stored after the page postback?](#where-the-viewstate-is-stored-after-the-page-postback)

[How long the items in ViewState exists?](#how-long-the-items-in-viewstate-exists)

[What are the different validators in ASP.NET? ](#what-are-the-different-validators-in-aspnet-)

[What is ViewState? How is it encoded? Is it encrypted? Who uses ViewState?](#what-is-viewstate-how-is-it-encoded-is-it-encrypted-who-uses-viewstate)

[List the events in ASP.NET page life cycle](#list-the-events-in-aspnet-page-life-cycle)

[Can we add code files of different languages in App_Code folder?](#can-we-add-code-files-of-different-languages-in-app_code-folder)

[How can we prevent browser from caching an ASPX page?](#how-can-we-prevent-browser-from-caching-an-aspx-page)

[In which event of page cycle is the ViewState available?](#in-which-event-of-page-cycle-is-the-viewstate-available)

[What are the event handlers that we can have in Global.asax file?](#what-are-the-event-handlers-that-we-can-have-in-globalasax-file)

[From which base class all Web Forms are inherited?](#from-which-base-class-all-web-forms-are-inherited)

[What is the difference between an HtmlInputCheckBox control and an HtmlInputRadioButton control?](#what-is-the-difference-between-an-htmlinputcheckbox-control-and-an-htmlinputradiobutton-control)

[In which event are the controls fully loaded?](#in-which-event-are-the-controls-fully-loaded)

[What is the difference between web config and machine config?](#what-is-the-difference-between-web-config-and-machine-config)

[What is RedirectPermanent in ASP.Net?](#what-is-redirectpermanent-in-aspnet)

[What are the different Session state management options available in ASP.NET?](#what-are-the-different-session-state-management-options-available-in-aspnet)

[List the major built-in objects in ASP.NET?](#list-the-major-built-in-objects-in-aspnet)

[Which type if caching will be used if we want to cache the portion of a page instead of whole page?](#which-type-if-caching-will-be-used-if-we-want-to-cache-the-portion-of-a-page-instead-of-whole-page)

[How can we apply Themes to an asp.net application?](#how-can-we-apply-themes-to-an-aspnet-application)

[What are the different types of cookies in ASP.NET?](#what-are-the-different-types-of-cookies-in-aspnet)

[How we can force all the validation controls to run?](#how-we-can-force-all-the-validation-controls-to-run)

[What is the difference between Web Service and WCF Service?](#what-is-the-difference-between-web-service-and-wcf-service)

[Is it possible to create web application with both webforms and mvc?](#is-it-possible-to-create-web-application-with-both-webforms-and-mvc)

[What is the difference between a web API and a web service?](#what-is-the-difference-between-a-web-api-and-a-web-service)

[What is Cross Page Posting?](#what-is-cross-page-posting)

[What is the equivalent of WebForms in ASP.NET Core?](#what-is-the-equivalent-of-webforms-in-aspnet-core)

[Name some ASP.NET WebForms disadvantages over MVC?](#name-some-aspnet-webforms-disadvantages-over-mvc)



### What is ViewData?

Viewdata contains the key, value pairs as dictionary and this is derived from class — “ViewDataDictionary“. In action method we are setting the value for viewdata and in view the value will be fetched by typecasting.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet)
### What is ASP.Net?

It is a framework developed by Microsoft on which we can develop new generation web sites using web forms(aspx), MVC, HTML, Javascript, CSS etc. Its successor of Microsoft Active Server Pages(ASP). Currently there is ASP.NET 4.0, which is used to develop web sites. There are various page extensions provided by Microsoft that are being used for web site development. Eg: aspx, asmx, ascx, ashx, cs, vb, html, XML etc. 


###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is ViewState?

**View State** is the method to preserve the Value of the Page and Controls between round trips. It is a Page-Level State Management technique. View State is turned on by default and normally serializes the data in every control on the page regardless of whether it is actually used during a post-back.  
  
A web application is stateless. That means that a new instance of a page is created every time when we make a request to the server to get the page and after the round trip our page has been lost immediately  

###### Source

* https://www.c-sharpcorner.com/UploadFile/8ef97c/Asp-Net-interview-questions-and-answers/

[[↑] Back to top](#aspnet)
### How you can add an event handler?

** **Using the Attributes property of server side control. 

e.g. 
```csharp
btnSubmit.Attributes.Add("onMouseOver","JavascriptCode();")
```

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What's the use of Response.Output.Write()?

We can write formatted output using Response.Output.Write(). 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the difference between ASP.NET and ASP.NET MVC?

ASP.NET, at its most basic level, provides a means for you to provide general HTML markup combined with server side "controls" within the event-driven programming model that can be leveraged with VB, C#, and so on. You define the page(s) of a site, drop in the controls, and provide the programmatic plumbing to make it all work.

ASP.NET MVC is an application framework based on the Model-View-Controller architectural pattern. This is what might be considered a "canned" framework for a specific way of implementing a web site, with a page acting as the "controller" and dispatching requests to the appropriate pages in the application. The idea is to "partition" the various elements of the application, eg business rules, presentation rules, and so on.

Think of the former as the "blank slate" for implementing a site architecture you've designed more or less from the ground up. MVC provides a mechanism for designing a site around a pre-determined "pattern" of application access, if that makes sense. There's more technical detail to it than that, to be sure, but that's the nickel tour for the purposes of the question.

###### Source

* https://stackoverflow.com/questions/12167401/what-is-the-difference-between-asp-net-and-asp-net-mvc

[[↑] Back to top](#aspnet)
### What is a postback?

A **postback** originates from the client browser. Usually one of the controls on the page will be manipulated by the user (a button clicked or dropdown changed, etc), and this control will initiate a postback. The state of this control, plus all other controls on the page (known as the View State) is Posted Back to the web server.

###### Source

* https://stackoverflow.com/questions/183254/what-is-a-postback

[[↑] Back to top](#aspnet)
### What is the good practice to implement validations in aspx page?

Client-side validation is the best way to validate data of a web page. It reduces the network traffic and saves server resources. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the file extension of ASP.NET web service?

Web services have file extension `.asmx`.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the meaning of Unobtrusive JavaScript?

This is a general term that conveys a general philosophy, similar to the term REST (Representational State Transfer). Unobtrusive JavaScript doesn’t intermix JavaScript code in your page markup.

Eg : Instead of using events like onclick and onsubmit, the unobtrusive JavaScript attaches to elements by their ID or class based on the HTML5 data- attributes.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet)
### Explain JSON Binding?

JavaScript Object Notation (JSON) binding support started from MVC3 onwards via the new JsonValueProviderFactory, which _allows the action methods to accept and model-bind data in JSON format_. This is useful in Ajax scenarios like client templates and data binding that need to post data back to the server.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet)
### What are the different types of caching?

ASP.NET has 3 kinds of caching : 

1. Output Caching,
2. Fragment Caching,
3. Data Caching.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What are the sub types of ActionResult?

ActionResult is used to represent the action method result. Below are the subtypes of ActionResult:

* ViewResult
* PartialViewResult
* RedirectToRouteResult
* RedirectResult
* JavascriptResult
* JSONResult
* FileResult
* HTTPStatusCodeResult

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet)
###  How do you register JavaScript for webcontrols?

We can register javascript for controls using `Attribtues.Add(scriptname,scripttext)` method. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the difference between Server.Transfer and Response.Redirect?

In Server.Transfer page processing transfers from one page to the other page without making a round-trip back to the client's browser. This provides a faster response with a little less overhead on the server. The clients url history list or current url Server does not update in case of Server.Transfer. 

Response.Redirect is used to redirect the user's browser to another page or site. It performs trip back to the client where the client's browser is redirected to the new page. The user's browser history list is updated to reflect the new address. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### Where the viewstate is stored after the page postback?

ViewState is stored in a hidden field on the page at client side. ViewState is transported to the client and back to the server, and is not stored on the server or any other external source. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### How long the items in ViewState exists?

They exist for the life of the current page.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What are the different validators in ASP.NET? 

**Client-Side Validation:** When validation is done on the client browser, then it is known as Client-Side Validation. We use JavaScript to do the Client-Side Validation.  
  
**Server-Side Validation: **  When validation occurs on the server, then it is known as Server-Side Validation. Server-Side Validation is a secure form of validation. The main advantage of Server-Side Validation is if the user somehow bypasses the Client-Side Validation, we can still catch the problem on server-side. 

###### Source

* https://www.c-sharpcorner.com/UploadFile/8ef97c/Asp-Net-interview-questions-and-answers/

[[↑] Back to top](#aspnet)
### What is ViewState? How is it encoded? Is it encrypted? Who uses ViewState?

**View state** is a kind of hash map (or at least you can think of it that way) that ASP.NET uses to store all the temporary information about a page - like what options are currently chosen in each select box, what values are there in each text box, which panel are open, etc. You can also use it to store any arbitrary information.

The entire map is serialized and encoded and kept in a _hidden variable_ (__VIEWSTATE form field) that's posted back to the server whenever you take any action on the page that requires a server round trip. This is how you can access the values on the controls from the server code. If you change any value in the server code, that change is made in the view state and sent back to the browser.

Just be careful about how much information you store in the view state, though... it can quickly become bloated and slow to transfer each time to the server and back.

It's not encrypted at all. Just base encoded, which easily reversible.

###### Source

* https://stackoverflow.com/questions/2305297/what-is-viewstate-how-is-it-encoded-is-it-encrypted-who-uses-viewstate

[[↑] Back to top](#aspnet)
### List the events in ASP.NET page life cycle

1) Page_PreInit  
2) Page_Init  
3) Page_InitComplete  
4) Page_PreLoad  
5) Page_Load  
6) Page_LoadComplete  
7) Page_PreRender  
8) Render

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### Can we add code files of different languages in App_Code folder?

No. The code files must be in same language to be kept in App_code folder.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### How can we prevent browser from caching an ASPX page?

We can SetNoStore on HttpCachePolicy object exposed by the Response object's Cache property: 
    
```csharp
Response.Cache.SetNoStore();
Response.Write(DateTime.Now.ToLongTimeString ());
```

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### In which event of page cycle is the ViewState available?

After the Init() and before the Page_Load(). 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What are the event handlers that we can have in Global.asax file?

* **Application Events:** Application_Start , Application_End, Application_AcquireRequestState, Application_AuthenticateRequest, Application_AuthorizeRequest, Application_BeginRequest, Application_Disposed, Application_EndRequest, Application_Error, Application_PostRequestHandlerExecute, Application_PreRequestHandlerExecute,Application_PreSendRequestContent, Application_PreSendRequestHeaders, Application_ReleaseRequestState, Application_ResolveRequestCache, Application_UpdateRequestCache 

* **Session Events:** Session_Start,Session_End 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### From which base class all Web Forms are inherited?

Page class.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the difference between an HtmlInputCheckBox control and an HtmlInputRadioButton control?

In `HtmlInputCheckBoxcontrol`, multiple item selection is possible whereas in `HtmlInputRadioButton` controls, we can select only single item from the group of items. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### In which event are the controls fully loaded?

**Page load** event. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the difference between web config and machine config?

Web config file is specific to a web application where as machine config is specific to a machine or server. There can be multiple web config files into an application where as we can have only one machine config file on a server. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is RedirectPermanent in ASP.Net?

**RedirectPermanent** Performs a permanent redirection from the requested URL to the specified URL. Once the redirection is done, it also returns 301 Moved Permanently responses. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What are the different Session state management options available in ASP.NET?

* **In-Process** stores the session in memory on the web server. 
* **Out-of-Process** Session state management stores data in an external server. The external server may be either a SQL Server or a State Server. All objects stored in session are required to be serializable for Out-of-Process state management. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### List the major built-in objects in ASP.NET?

* Application 
* Request 
* Response 
* Server 
* Session 
* Context 
* Trace 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### Which type if caching will be used if we want to cache the portion of a page instead of whole page?

**Fragment Caching:** It caches the portion of the page generated by the request. For that, we can create user controls with the below code: 

```html    
<%@ OutputCache Duration="120" VaryByParam="CategoryID;SelectedID"%>
```

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### How can we apply Themes to an asp.net application?

We can specify the theme in web.config file.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What are the different types of cookies in ASP.NET?

* **Session Cookie** \- Resides on the client machine for a single session until the user does not log out. 
* **Persistent Cookie** \- Resides on a user's machine for a period specified for its expiry, such as 10 days, one month, and never. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### How we can force all the validation controls to run?

The `Page.Validate()` method is used to force all the validation controls to run and to perform validation.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the difference between Web Service and WCF Service?

* Web Service is based on SOAP and return data in XML form. It support only HTTP/S protocol. It is not open source but can be consumed by any client that understands xml. It can be hosted only on IIS.

* WCF is also based on SOAP and return data in XML form. It is the evolution of the web service(ASMX) and support various protocols like TCP, HTTP, HTTPS, Named Pipes, MSMQ. The main issue with WCF is, its tedious and extensive configuration. It is not open source but can be consumed by any client that understands xml. It can be hosted with in the applicaion or on IIS or using window service.

###### Source

* https://stackoverflow.com/questions/351334/web-service-vs-wcf-service

[[↑] Back to top](#aspnet)
### Is it possible to create web application with both webforms and mvc?

Yes. We have to include below mvc assembly references in the web forms application to create hybrid application. 

* System.Web.Mvc
* System.Web.Razor
* System.ComponentModel.DataAnnotations

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the difference between a web API and a web service?

* A web service typically offers a WSDL from which you can create client stubs automatically. Web Services are based on the SOAP protocol. 

* ASP.NET Web API is a newer Microsoft framework which helps you to build REST based interfaces. The response can be either JSON or XML, but there is no way to generate clients automatically because Web API does not offer a service description like the WSDL from Web Services. 

###### Source

* https://stackoverflow.com/questions/19336347/what-is-the-difference-between-a-web-api-and-a-web-service

[[↑] Back to top](#aspnet)
### What is Cross Page Posting?

When we click submit button on a web page, the page post the data to the same page. The technique in which we post the data to different pages is called Cross Page posting. This can be achieved by setting POSTBACKURL property of the button that causes the postback. Findcontrol method of PreviousPage can be used to get the posted values on the page to which the page has been posted. 

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### What is the equivalent of WebForms in ASP.NET Core?

ASP.NET Core Razor Pages is the modern equivalent to "Classic ASP.NET Web Forms." Razor Pages is a new aspect of ASP.NET Core MVC that makes coding page-focused scenarios easier and more productive.

###### Source

* https://www.guru99.com/asp-net-interview-questions-answers.html

[[↑] Back to top](#aspnet)
### Name some ASP.NET WebForms disadvantages over MVC?

MVC is almost ALWAYS the better solution. There is why:

* The page lifecylce is simpler and more efficient
* There is no such thing as controls besides html controls. You don't need to debug your output to see what ASP .Net is generating.
* ViewModels give you immense power and obviate the need to do manual control binding and it eliminates many errors relating to binding.
* You can have multiple forms on a page. This was a serious limitation of WebForms.
* The web is stateless and MVC matches the architecture of the web more closely. Webforms introduces state and the bugs you have with it by introducing the ViewState. The ViewState is automatic and works in the background, so it doesn't always behave the way you want it to.
* Web applications need to work with ajax these days. It's not acceptable to have full page loads any more. MVC makes ajax so so much better, easier and more efficient with JQuery.
* Because you can have multiple forms on a page, and because the architecture is driven by calls to urls, you can do funky things like ajax load a different form, like an edit form into your current page using JQuery. Once you realise what this lets you do you can do amazing things easily.
* ASP.Net WebForms is not only an abstraction over html, it is an extremely complex one. Sometimes you would get a weird bug and struggle with it for much longer than need be. In many cases you could actually see what it was doing wrong but you are unable to do anything about it. You end up doing weird workarounds.
* WebForms does not make a good technology for designers. Designers often like working with html directly. In MVC it's a view, in WebForms it's half a day of work.
* As the web platform is evolving fast WebForms wont keep up. It's not aware of new tags or features of HTML5, it will still render the same stuff unless you get (often) expensive 3rd party controls or wait for Microsoft to issue an update.
* Controls in WebForms limit you in so many ways. In MVC you can just grab a JQuery library and integrate it into your templates.

###### Source

* https://softwareengineering.stackexchange.com/questions/95212/when-to-favor-asp-net-webforms-over-mvc

[[↑] Back to top](#aspnet)
