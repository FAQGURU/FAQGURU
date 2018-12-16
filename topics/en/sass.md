## Sass

[How to use variables in Sass?](#how-to-use-variables-in-sass)

[What Selector Nesting in Sass is used for?](#what-selector-nesting-in-sass-is-used-for)

[List out the key features for Sass?](#list-out-the-key-features-for-sass)

[What is variable interpolation in Sass? Provide some examples. ](#what-is-variable-interpolation-in-sass-provide-some-examples-)

[List out the data types that Sass supports](#list-out-the-data-types-that-sass-supports)

[What is Sass?](#what-is-sass)

[Explain what is a @extend directive used for in Sass?](#explain-what-is-a-extend-directive-used-for-in-sass)

[What's the difference between SCSS and Sass?](#whats-the-difference-between-scss-and-sass)

[What is a Mixin and how to use on?](#what-is-a-mixin-and-how-to-use-on)

[What will be the CSS output for the following Sass code?](#what-will-be-the-css-output-for-the-following-sass-code)

[What is the '@content' directive used for?](#what-is-the-content-directive-used-for)

[What’s wrong with Sass nesting? Provide some example.](#whats-wrong-with-sass-nesting-provide-some-example)



### How to use variables in Sass?

Think of variables as a way to store information that you want to reuse throughout your stylesheet. You can store things like colors, font stacks, or any CSS value you think you'll want to reuse. Sass uses the `$` symbol to make something a variable.

```css
$font-stack:    Helvetica, sans-serif;
$primary-color: #333;

body {
  font: 100% $font-stack;
  color: $primary-color;
}
```


###### Source

* https://sass-lang.com/guide

[[↑] Back to top](#Sass)
### What Selector Nesting in Sass is used for?

Sass *let you nest* your CSS selectors in a way that follows the same visual hierarchy of your HTML.  CSS, on the other hand, doesn't have any visual hierarchy.

Consider example (scss):
```css
.parent {
  color: red;

  .child {
    color: blue;
  }
}
```
Result (css):
```css
.parent {
  color: red;
}

.parent .child {
  color: blue;
}
```


###### Source

* https://sass-lang.com/guide

[[↑] Back to top](#Sass)
### List out the key features for Sass?

Key features for Sass include

* Full CSS3-compatible
* Language extensions such as nesting, variables, and mixins
* Many useful functions for manipulating colors and other values
* Advanced features like control directives for libraries
* Well-formatted, customizable output

###### Source

* https://career.guru99.com/top-17-sass-interview-questions/

[[↑] Back to top](#Sass)
### What is variable interpolation in Sass? Provide some examples. 

 If you want to use variables inside a string, you will have to use a process called **variable interpolation**. To use it you will have to wrap your variables in `#{}`. 

Consider:
```css
$name: 'Gajendar';
$author: 'Author : $name'; // 'Author : $name'

$author: 'Author : #{$name}';
// 'Author : Gajendar'
```

The interpolation method could be useful in situations where the value of a variable is determined by some conditional statements. 

###### Source

* https://www.sitepoint.com/data-types-in-sass/

[[↑] Back to top](#Sass)
### List out the data types that Sass supports

Sass supports seven main data types:

* **Numbers** - most of the time they are accompanied by a unit of some sort but they are still technically numbers. You can perform basic mathematical operations on these values.

```css
$size: 18;                  // A number
$px-unit: $size * 1px;      // A pixel measurement
$px-string: $size + px;     // A string
$px-number: $px-unit / 1px; // A number
```
* **Strings** - just like CSS, accepts both quoted and unquoted strings, even if they contain spaces

```css
$website: 'SitePoint'; // Stores SitePoint
$name: 'Gajendar' + ' Singh';  // 'Gajendar Singh'
$date:  'Month/Year : ' + 3/2016; // 'Month/Year : 3/2016'
$date:  'Month/Year : ' + (3/2016); // 'Month/Year : 0.00149' 
// This is because 3/2016 is evaluated first.
$variable: 3/2016;      // Evaluated to 0.00149
```
* **Colors** - CSS color expressions come under the `color` data type. You can refer to the colors in hexadecimal notation, as `rgb`, `rgba`, `hsl` and `hsla` values or use native keywords like `pink`, `blue`, etc. 

```css
$color: yellowgreen;           // #9ACD32
color: lighten($color, 15%);    // #b8dc70
color: darken($color, 15%);     // #6c9023
color: saturate($color, 15%);   // #a1e01f
color: desaturate($color, 15%); // #93ba45
color: (green + red);           // #ff8000
```
* **Booleans** - has only two possible values: `true` and `false`

```css
$i-am-true: true;

body {
  @if not $i-am-true {
    background: rgba(255, 0, 0, 0.6);
  } @else {
    background: rgba(0, 0, 255, 0.6); // expected
  }
}
```

* **Null** -  is commonly used to define an empty state, neither `true` or `false`. This is typically the value you want to set when defining a variable without a value, only to prevent the parser from crashing.

```css
.foo {
  content: type-of(null); // null
  content: type-of(NULL); // string
  $bar: 'foo' + null; // invalid null operation: "foo plus null”.
}
```

* **Lists** - are just the Sass version of arrays. You can store multiple types of values in a list.

```css
$font-list: 'Raleway','Dosis','Lato'; // Three comma separated elements
$pad-list: 10px 8px 12px; // Three space separated elements
$multi-list: 'Roboto',15px 1.3em; // This multi-list has two lists.
```
* **Maps** -  Sass maps are like associative arrays. A map stores both keys and values associated with those keys.

```css
$styling: (
  'font-family': 'Lato',
  'font-size': 1.5em,
  'color': tomato,
  'background': black
);

h1 {
  color: map-get($styling, 'color');
  background: map-get($styling, 'background');
}
```

###### Source

* https://career.guru99.com/top-17-sass-interview-questions/

[[↑] Back to top](#Sass)
### What is Sass?

**Sass** or **Syntactically Awesome StyleSheets** is a *CSS* preprocessor that adds power and elegance to the basic language. It allows you to use variables, nested rules, mixins, inline imports, and more, all with a fully CSS-compatible syntax. Sass helps keep large stylesheets well-organized, and get small stylesheets up and running quickly.

A *CSS preprocessor* is a scripting language that extends CSS by allowing developers to write code in one language and then compile it into CSS. 


###### Source

* https://sass-lang.com/documentation/file.SASS_REFERENCE.html#syntax

[[↑] Back to top](#Sass)
### Explain what is a @extend directive used for in Sass?

Using `@extend` lets you share a set of CSS properties from one selector to another. It helps keep your Sass very dry.

Consider:
```css
%message-shared {
  border: 1px solid #ccc;
  padding: 10px;
  color: #333;
}

.message {
  @extend %message-shared;
}

.success {
  @extend %message-shared;
  border-color: green;
}

.error {
  @extend %message-shared;
  border-color: red;
}

.warning {
  @extend %message-shared;
  border-color: yellow;
}
```
CSS output:
```css
.message, .success, .error, .warning {
  border: 1px solid #cccccc;
  padding: 10px;
  color: #333;
}

.success {
  border-color: green;
}

.error {
  border-color: red;
}

.warning {
  border-color: yellow;
}
```

 

###### Source

* https://sass-lang.com/guide

[[↑] Back to top](#Sass)
### What's the difference between SCSS and Sass?

There are two syntaxes available for Sass. The first, known as **SCSS (Sassy CSS)** and used throughout this reference, is an extension of the syntax of CSS. This means that every valid CSS stylesheet is a valid SCSS file with the same meaning. This syntax is enhanced with the Sass features described below. Files using this syntax have the `.scss` extension.

The second and older syntax, known as the indented syntax (or sometimes just **Sass**), provides a more concise way of writing CSS. It uses indentation rather than brackets to indicate nesting of selectors, and newlines rather than semicolons to separate properties. Files using this syntax have the `.sass` extension.

Consider **example.sass**:
```css
$color: red

=my-border($color)
  border: 1px solid $color

body
  background: $color
  +my-border(green)
```

Consider **example.scss**:
```css
$color: red;

@mixin my-border($color) {
  border: 1px solid $color;
}

body {
  background: $color;
  @include my-border(green);
}
```


###### Source

* https://stackoverflow.com/questions/5654447/whats-the-difference-between-scss-and-sass

[[↑] Back to top](#Sass)
### What is a Mixin and how to use on?

A **Mixin** is a block of code that lets us group CSS declarations we may reuse throughout our site.

To define mixin:
```css
@mixin grid($flex: true /*default argument*/) {
    @if $flex {
        @include flex;
    } @else {
        display: block;
    }
}
```

To use a Mixin, we simply use `@include` followed by the name of the Mixin and a semi-colon.
```css
/*scss*/
.row {
    @include grid(true);
}

/*css*/
.row {
    display: -webkit-flex;
    display: flex;
}
```

###### Source

* https://scotch.io/tutorials/how-to-use-sass-mixins

[[↑] Back to top](#Sass)
### What will be the CSS output for the following Sass code?

Consider *Scss*:
```css
$style1: 100%, 70px, #fo6d06; // list
$style2: (background: #bada55, width: 100%, height: 100px); // map

@mixin box($width, $height, $background) {
    width: $width;
    height: $height;
    background-color: $background;
}

.fogdog {
    @include box($style1...); // use spread operator for the argument
}

.badass {
    @include box($style2...); // same for the map
}
```
Compiled *CSS*:
```css
.fogdog {
    width: 100%;
    height: 70px;
    background-color: #fo6d06;
}

.badass {
    width: 100%;
    height: 100px;
    background-color: #bada55;
}
```

###### Source

* https://scotch.io/tutorials/how-to-use-sass-mixins

[[↑] Back to top](#Sass)
### What is the '@content' directive used for?

`@content` allows for Mixin extension. We can pass a block to Mixins with the use of `@content`.

Consider mixin:
```css
@mixin small() {
    @media only screen and (max-width: 320px) {
        @content;
    }
}```
Instead of having to type the media query everytime, this feels like a much more stable way to handle media queries:
```css
@include small {
    // css code for small screens go here
}
```

###### Source

* https://scotch.io/tutorials/how-to-use-sass-mixins

[[↑] Back to top](#Sass)
### What’s wrong with Sass nesting? Provide some example.

In itself, there’s absolutely nothing wrong with nesting. The feature makes sense. The problem, as is often the case, is not the feature but how we use it.

* Nesting makes code complicated. For example:

```css
.tabs {
  .tab {
    background: red;

    &:hover {
      background: white;
    }

    .tab-link {
      color: white;

      @at-root #{selector-replace(&, '.tab', '.tab:hover')} { // @at-root jump out at the top level
        color: red;
      }
    }
  }
}
```
* The Reference selector `&` is ambiguous, depending on the way it is used, it can yield a totally different CSS output. For example:

```css
/* SCSS */
.element {
  &:hover {
    color: red;
  }
}

/* CSS */
.element:hover {
  color: red;
}
```
and:
```css
/* SCSS */
.element {
  & .hover {
    color: red;
  }
}

/* CSS */
.element .hover {
  color: red;
}
```

* Unsearchable selectors. Consider:

```css
.block {
  /* Some CSS declarations */

  &--modifier {
    /* Some CSS declarations for the modifier */
  }

  &__element {
    /* Some CSS for the element */

    &--modifier {
      /* Some CSS for the modifier of the element */
    }
  }
}
```
What if a developer wants to find the CSS from .block__element?

###### Source

* https://www.sitepoint.com/beware-selector-nesting-sass/

[[↑] Back to top](#Sass)
