## ASP.NET MVC

[What is Layout in MVC?](#what-is-layout-in-mvc)

[What are Actions in MVC?](#what-are-actions-in-mvc)

[What is Razor View Engine?](#what-is-razor-view-engine)

[What is the use of ViewModel in MVC?](#what-is-the-use-of-viewmodel-in-mvc)

[What you mean by Routing in MVC?](#what-you-mean-by-routing-in-mvc)

[What are the advantages of MVC over ASP.NET?](#what-are-the-advantages-of-mvc-over-aspnet)

[What are Scaffold templates in MVC?](#what-are-scaffold-templates-in-mvc)

[Explain Bundle.Config in MVC4?](#explain-bundleconfig-in-mvc4)

[Can you explain Model, Controller and View in MVC?](#can-you-explain-model-controller-and-view-in-mvc)

[Explain Sections is MVC?](#explain-sections-is-mvc)

[What are Non Action methods in MVC?](#what-are-non-action-methods-in-mvc)

[What is RouteConfig.cs in MVC 4?](#what-is-routeconfigcs-in-mvc-4)

[What is the difference between ViewBag and ViewData in MVC?](#what-is-the-difference-between-viewbag-and-viewdata-in-mvc)

[What is the "HelperPage.IsAjax" Property?](#what-is-the-helperpageisajax-property)

[What are HTML Helpers in MVC?](#what-are-html-helpers-in-mvc)

[Can you explain the page life cycle of MVC?](#can-you-explain-the-page-life-cycle-of-mvc)

[What is Attribute Routing in MVC?](#what-is-attribute-routing-in-mvc)

[What is PartialView in MVC?](#what-is-partialview-in-mvc)

[Can you explain RenderBody and RenderPage in MVC?](#can-you-explain-renderbody-and-renderpage-in-mvc)

[Explain the methods used to render the views in MVC?](#explain-the-methods-used-to-render-the-views-in-mvc)

[Explain ASP.NET WebApi vs MVC?](#explain-aspnet-webapi-vs-mvc)

[Can a view be shared across multiple controllers? If Yes, How we can do that?](#can-a-view-be-shared-across-multiple-controllers-if-yes-how-we-can-do-that)

[Explain TempData in MVC?](#explain-tempdata-in-mvc)

[What are Validation Annotations?](#what-are-validation-annotations)

[Why to use Html.Partial in MVC?](#why-to-use-htmlpartial-in-mvc)

[How route table has been created in ASP.NET MVC?](#how-route-table-has-been-created-in-aspnet-mvc)

[Explain Dependency Resolution?](#explain-dependency-resolution)

[What is Separation of Concerns in ASP.NET MVC?](#what-is-separation-of-concerns-in-aspnet-mvc)

[What are AJAX Helpers in MVC?](#what-are-ajax-helpers-in-mvc)

[What is Html.RenderPartial?](#what-is-htmlrenderpartial)



### What is Layout in MVC?

Layout pages are similar to master pages in traditional web forms. This is used to set the common look across multiple pages. In each child page we can find —

```html
@{
Layout = “~/Views/Shared/TestLayout1.cshtml”;
}
```

This indicates child page uses TestLayout page as it’s master page.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What are Actions in MVC?

**Actions** are the methods in Controller class which is responsible for returning the view or json data. Action will mainly have return type — “ActionResult” and it will be invoked from method — “InvokeAction()” called by controller.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is Razor View Engine?

**Razor** is the first major update to render HTML in MVC 3. Razor was designed specifically for view engine syntax. Main focus of this would be to simplify and code-focused templating for HTML generation. Below is the sample of using Razor:

```html
@model MvcMusicStore.Models.Customer
@{ViewBag.Title = “Get Customers”;}
<div class=”cust”> <h3><em>@Model.CustomerName</em> </h3>
```


###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is the use of ViewModel in MVC?

ViewModel is a plain class with properties, which is used to bind it to strongly typed view. ViewModel can have the validation rules defined for its properties using data annotations.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What you mean by Routing in MVC?

**Routing** is a pattern matching mechanism of incoming requests to the URL patterns which are registered in route table. Class — “UrlRoutingModule” is used for the same process.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What are the advantages of MVC over ASP.NET?

* Provides a clean separation of concerns among UI (Presentation layer), model (Transfer objects/Domain Objects/Entities) and Business Logic (Controller).
* Easy to UNIT Test
* Improved reusability of model and views. We can have multiple views which can point to the same model and vice versa.
* Improved structuring of the code

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What are Scaffold templates in MVC?

Scaffolding in ASP.NET MVC is used to generate the Controllers, Model and Views for create, read, update, and delete (CRUD) functionality in an application. The scaffolding will be knowing the naming conventions used for models and controllers and views.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Explain Bundle.Config in MVC4?

**“BundleConfig.cs”** in MVC4 is used to register the bundles by the bundling and minification system. Many bundles are added by default including jQuery libraries like — jquery.validate, Modernizr, and default CSS references.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Can you explain Model, Controller and View in MVC?

* **Model** — It’s a business entity and it is used to represent the application data.
* **Controller** — Request sent by the user always scatters through controller and it’s responsibility is to redirect to the specific view using View() method.
* **View** — It’s the presentation layer of MVC.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Explain Sections is MVC?

Section are the part of HTML which is to be rendered in layout page. In Layout page we will use the below syntax for rendering the HTML –

```html
@RenderSection(“TestSection”)
```

And in child pages we are defining these sections as shown below –

```html
@section TestSection{
     <h1>Test Content</h1>
}
```

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What are Non Action methods in MVC?

In MVC all public methods have been treated as Actions. So if you are creating a method and if you do not want to use it as an action method then the method has to be decorated with "NonAction" attribute as shown below:

```csharp
[NonAction]
public void TestMethod()
{
   // Method logic
}
```

###### Source

* https://stackoverflow.com/questions/21758615/why-should-i-use-ihttpactionresult-instead-of-httpresponsemessage

[[↑] Back to top](#aspnet-mvc)
### What is RouteConfig.cs in MVC 4?

"RouteConfig.cs" holds the routing configuration for MVC. RouteConfig will be initialized on Application_Start event registered in Global.asax.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is the difference between ViewBag and ViewData in MVC?

ViewBag is a wrapper around ViewData, which allows to create dynamic properties. Advantage of viewbag over viewdata will be:
* In ViewBag no need to typecast the objects as in ViewData.
* ViewBag will take advantage of dynamic keyword which is introduced in version 4.0. But before using ViewBag we have to keep in mind that ViewBag is slower than ViewData.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is the "HelperPage.IsAjax" Property?

The HelperPage.IsAjax property gets a value that indicates whether Ajax is being used during the request of the Web page.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What are HTML Helpers in MVC?

HTML Helpers are like controls in traditional web forms. But HTML helpers are more lightweight compared to web controls as it does not hold viewstate and events.
HTML Helpers returns the HTML string which can be directly rendered to HTML page. Custom HTML Helpers also can be created by overriding “HtmlHelper” class.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Can you explain the page life cycle of MVC?

Below are the processed followed in the sequence:
* App initialization
* Routing
* Instantiate and execute controller
* Locate and invoke controller action
* Instantiate and render view


###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is Attribute Routing in MVC?

ASP.NET Web API supports this type routing. This is introduced in MVC5. In this type of routing, attributes are being used to define the routes. This type of routing gives more control over classic URI Routing. Attribute Routing can be defined at controller level or at Action level like –

```js
[Route(“{action = TestCategoryList}”)] — Controller Level
[Route(“customers/{TestCategoryId:int:min(10)}”)] — Action Level
```

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is PartialView in MVC?

PartialView is similar to UserControls in traditional web forms. For re-usability purpose partial views are used. Since it's been shared with multiple views these are kept in shared folder. Partial Views can be rendered in following ways –

* Html.Partial()
* Html.RenderPartial()

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Can you explain RenderBody and RenderPage in MVC?

RenderBody is like ContentPlaceHolder in web forms. This will exist in layout page and it will render the child pages/views. Layout page will have only one RenderBody() method. RenderPage also exists in Layout page and multiple RenderPage() can be there in Layout page.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Explain the methods used to render the views in MVC?

Below are the methods used to render the views from action:

* View() — To return the view from action.
* PartialView() — To return the partial view from action.
* RedirectToAction() — To Redirect to different action which can be in same controller or in different controller.
* Redirect() — Similar to “Response.Redirect()” in webforms, used to redirect to specified URL.
* RedirectToRoute() — Redirect to action from the specified URL but URL in the route table has been matched.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Explain ASP.NET WebApi vs MVC?

Usually, WebAPI used for data services where MVC can generate more types of outputs (like template HTML views).

* WebAPI simplifies the way we can create REST data services. It's clean and easy for this purpose.
* MVC can generate any output WebAPI can output. Generating outputs from templates can be easily achieved in MVC. I can't find a reason to do so in WebAPI. 

###### Source

* https://stackoverflow.com/questions/19336347/what-is-the-difference-between-a-web-api-and-a-web-service

[[↑] Back to top](#aspnet-mvc)
### Can a view be shared across multiple controllers? If Yes, How we can do that?

Yes, we can share a view across multiple controllers. We can put the view in the "Shared" folder. When we create a new MVC Project we can see the Layout page will be added in the shared folder, which is because it is used by multiple child pages.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Explain TempData in MVC?

TempData is again a key, value pair as ViewData. This is derived from “TempDataDictionary” class. TempData is used when the data is to be used in two consecutive requests, this could be between the actions or between the controllers. This requires typecasting in view.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What are Validation Annotations?

**Data annotations** are attributes which can be found in the "System.ComponentModel.DataAnnotations" namespace. These attributes will be used for server-side validation and client-side validation is also supported. Four attributes — Required, String Length, Regular Expression and Range are used to cover the common validation scenarios.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Why to use Html.Partial in MVC?

This method is used to render the specified partial view as an HTML string. This method does not depend on any action methods. We can use this like below:

```html
@Html.Partial("TestPartialView")
```

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### How route table has been created in ASP.NET MVC?

Method — “RegisterRoutes()” is used for registering the routes which will be added in “Application_Start()” method of global.asax file, which is fired when the application is loaded or started.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### Explain Dependency Resolution?

**Dependency Resolver** has been introduced in MVC3 and it is greatly simplified the use of dependency injection in your applications. This turn to be easier and useful for decoupling the application components and making them easier to test and more configurable.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is Separation of Concerns in ASP.NET MVC?

It’s is the process of breaking the program into various distinct features which overlaps in functionality as little as possible. MVC pattern concerns on separating the content from presentation and data-processing from content.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What are AJAX Helpers in MVC?

AJAX Helpers are used to create AJAX enabled elements like as Ajax enabled forms and links which performs the request asynchronously and these are extension methods of AJAXHelper class which exists in namespace — System.Web.Mvc.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
### What is Html.RenderPartial?

Result of the method — "RenderPartial" is directly written to the HTML response. This method does not return anything (void). This method also does not depend on action methods. RenderPartial() method calls "Write()" internally and we have to make sure that "RenderPartial" method is enclosed in the bracket.

###### Source

* https://medium.com/dot-net-tutorial/top-50-asp-net-mvc-interview-questions-with-answers-1fd9b1638c61

[[↑] Back to top](#aspnet-mvc)
