## CSS

[Explain the three main ways to apply CSS styles to a web page](#explain-the-three-main-ways-to-apply-css-styles-to-a-web-page)

[What is CSS?](#what-is-css)

[What is DOM (Document Object Model) and how is it linked to CSS?](#what-is-dom-document-object-model-and-how-is-it-linked-to-css)

[Explain the CSS “box model” and the layout components that it consists of](#explain-the-css-box-model-and-the-layout-components-that-it-consists-of)

[What is a CSS rule?](#what-is-a-css-rule)

[What existing CSS frameworks have you used locally, or in production? How would you change/improve them?](#what-existing-css-frameworks-have-you-used-locally-or-in-production-how-would-you-changeimprove-them)

[Have you played around with the new CSS Flexbox or Grid specs?](#have-you-played-around-with-the-new-css-flexbox-or-grid-specs)

[What is the difference between classes and IDs in CSS?](#what-is-the-difference-between-classes-and-ids-in-css)

[Describe floats and how they work](#describe-floats-and-how-they-work)

[Explain CSS sprites, and how you would implement them on a page or site.](#explain-css-sprites-and-how-you-would-implement-them-on-a-page-or-site)

[How would you approach fixing browser-specific styling issues?](#how-would-you-approach-fixing-browser-specific-styling-issues)

[What is CSS preprocessor and why to user one?](#what-is-css-preprocessor-and-why-to-user-one)

[Have you ever worked with retina graphics? If so, when and what techniques did you use?](#have-you-ever-worked-with-retina-graphics-if-so-when-and-what-techniques-did-you-use)

[How is responsive design different from adaptive design?](#how-is-responsive-design-different-from-adaptive-design)

[How to create a zebra striped table with CSS?](#how-to-create-a-zebra-striped-table-with-css)

[What’s the difference between “resetting” and “normalizing” CSS? Which would you choose, and why?](#whats-the-difference-between-resetting-and-normalizing-css-which-would-you-choose-and-why)

[How does CSS actually work (under the hood of browser)?](#how-does-css-actually-work-under-the-hood-of-browser)

[Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.](#explain-your-understanding-of-the-box-model-and-how-you-would-tell-the-browser-in-css-to-render-your-layout-in-different-box-models)

[What is CSS selectors? Name some.](#what-is-css-selectors-name-some)

[Explain the usage of "table-layout" property](#explain-the-usage-of-table-layout-property)

[Describe pseudo-elements and discuss what they are used for.](#describe-pseudo-elements-and-discuss-what-they-are-used-for)

[What does Accessibility (a11y) mean?](#what-does-accessibility-a11y-mean)

[What are the advantages/disadvantages of using CSS preprocessors?](#what-are-the-advantagesdisadvantages-of-using-css-preprocessors)

[What is a Grid System in CSS?](#what-is-a-grid-system-in-css)

[What's the difference between a `relative`, `fixed`, `absolute` and `static`ally positioned element?](#whats-the-difference-between-a-relative-fixed-absolute-and-statically-positioned-element)

[Explain the purpose of clearing floats in CSS](#explain-the-purpose-of-clearing-floats-in-css)

[How do you optimize your webpages for print?](#how-do-you-optimize-your-webpages-for-print)

[Have you ever used a grid system, and if so, what do you prefer?](#have-you-ever-used-a-grid-system-and-if-so-what-do-you-prefer)

[What are the different ways to visually hide content (and make it available only for screen readers)?](#what-are-the-different-ways-to-visually-hide-content-and-make-it-available-only-for-screen-readers)

[Describe z-index and how a stacking context is formed](#describe-z-index-and-how-a-stacking-context-is-formed)

[What does * { box-sizing: border-box; } do? What are its advantages?](#what-does---box-sizing-border-box--do-what-are-its-advantages)

[Can you explain the difference between coding a website to be responsive versus using a mobile-first strategy?](#can-you-explain-the-difference-between-coding-a-website-to-be-responsive-versus-using-a-mobile-first-strategy)

[Explain the basic rules of CSS Specificity](#explain-the-basic-rules-of-css-specificity)

[Is there any reason you'd want to use `translate()` instead of `absolute` positioning, or vice-versa? And why?](#is-there-any-reason-youd-want-to-use-translate-instead-of-absolute-positioning-or-vice-versa-and-why)

[What the code fragment has the greater CSS specificity? ](#what-the-code-fragment-has-the-greater-css-specificity-)

[What clearfix methods do you know? Provide some examples.](#what-clearfix-methods-do-you-know-provide-some-examples)

[How to style every element which has an adjacent item right before it?](#how-to-style-every-element-which-has-an-adjacent-item-right-before-it)

[Write down a selector that will match any links end in .zip, .ZIP, .Zip etc...](#write-down-a-selector-that-will-match-any-links-end-in-zip-zip-zip-etc)



### Explain the three main ways to apply CSS styles to a web page

Using the inline style attribute on an element
```html
<div>
    <p style="color: maroon;"></p>
</div>
```
Using a `<style>` block in the `<head>` section of your HTML
```html
<head>
    <title>CSS Refresher</title>
    <style>
        body {
            font-family: sans-serif;
            font-size: 1.2em;
        }
    </style>
</head>
```
Loading an external CSS file using the `<link>` tag
```html
<head>
    <title>CSS Refresher</title>
    <link rel="stylesheet" href="/css/styles.css" />
</head>
```

###### Source

* https://www.goskills.com/Development/Articles/CSS-interview-questions-answers

[[↑] Back to top](#CSS)
### What is CSS?

**CSS** stands for **Cascading Style Sheets**. CSS is used to define styles for your web pages, including the design, layout and variations in display for different devices and screen sizes.

CSS was intended to allow web professionals to separate the content and structure of a website's code from the visual design.

###### Source

* https://www.w3schools.com/css/css_intro.asp

[[↑] Back to top](#CSS)
### What is DOM (Document Object Model) and how is it linked to CSS?

The *Document Object Model (DOM)* is a cross-platform and language-independent *application programming interface* that treats an HTML, XHTML, or XML document as a tree structure wherein each node is an object representing a part of the document. 

With the Document Object Model, programmers can create and build documents, navigate their structure, and add, modify, or delete elements and content. The DOM specifies interfaces which may be used to manage XML or HTML documents. 

When a browser displays a document, it must combine the document's content with its style information. The browser converts HTML and CSS into the DOM (Document Object Model). The DOM represents the document in the computer's memory. It combines the document's content with its style.

###### Source

* https://en.wikipedia.org/wiki/Document_Object_Model

[[↑] Back to top](#CSS)
### Explain the CSS “box model” and the layout components that it consists of

The CSS box model is a rectangular layout paradigm for HTML elements that consists of the following:

* **Content** - The content of the box, where text and images appear
* **Padding** - A transparent area surrounding the content (i.e., the amount of space between the border and the content)
* **Border** - A border surrounding the padding (if any) and content
* **Margin** - A transparent area surrounding the border (i.e., the amount of space between the border and any neighboring elements)

###### Source

* https://www.toptal.com/css/interview-questions

[[↑] Back to top](#CSS)
### What is a CSS rule?

Web browsers apply **CSS rules** to a document to affect how they are displayed. A CSS rule is formed from:

* A **set of properties**, which have values set to update how the HTML content is displayed,
* A **selector**, which selects the element(s) you want to apply the updated property values to.

A set of CSS rules contained within a stylesheet determines how a webpage should look. 

###### Source

* https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/How_CSS_works

[[↑] Back to top](#CSS)
### What existing CSS frameworks have you used locally, or in production? How would you change/improve them?

* **Bootstrap** - Slow release cycle. Bootstrap 4 has been in alpha for almost 2 years. Add a spinner button component, as it is widely used.
* **Semantic UI** - Source code structure makes theme customization extremely hard to understand. Its unconventional theming system is a pain to customize. Hardcoded config path within the vendor library. Not well-designed for overriding variables unlike in Bootstrap.
* **Bulma** - A lot of non-semantic and superfluous classes and markup required. Not backward compatible. Upgrading versions breaks the app in subtle manners.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### Have you played around with the new CSS Flexbox or Grid specs?

Yes. Flexbox is mainly meant for 1-dimensional layouts while Grid is meant for 2-dimensional layouts.

Flexbox solves many common problems in CSS, such as vertical centering of elements within a container, sticky footer, etc. Bootstrap and Bulma are based on Flexbox, and it is probably the recommended way to create layouts these days. Have tried Flexbox before but ran into some browser incompatibility issues (Safari) in using `flex-grow`, and I had to rewrite my code using `inline-blocks` and math to calculate the widths in percentages, it wasn't a nice experience.

Grid is by far the most intuitive approach for creating grid-based layouts (it better be!) but browser support is not wide at the moment.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### What is the difference between classes and IDs in CSS?

* **IDs** — Meant to be unique within the document. Can be used to identify an element when linking using a fragment identifier. Elements can only have one id attribute.

* **Classes** — Can be reused on multiple elements within the document. Mainly for styling and targeting elements.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### Describe floats and how they work

*Float* is a CSS positioning property. Floated elements remain a part of the flow of the web page. This is distinctly different than page elements that use absolute positioning. Absolutely positioned page elements are removed from the flow of the webpage.

```css
#sidebar {
  float: right; // left right none inherit			
}
```
The CSS clear property can be used to be positioned below `left`/`right`/`both` floated elements.

###### Source

* https://css-tricks.com/all-about-floats/

[[↑] Back to top](#CSS)
### Explain CSS sprites, and how you would implement them on a page or site.

*CSS sprites* combine multiple images into one single larger image. It is commonly used technique for icons (Gmail uses it). 

* Use a sprite generator that packs multiple images into one and generate the appropriate CSS for it.
* Each image would have a corresponding CSS class with `background-image`, `background-position` and `background-size` properties defined.
* To use that image, add the corresponding class to your element.

**Advantages**:

* Reduce the number of HTTP requests for multiple images (only one single request is required per spritesheet). But with HTTP2, loading multiple images is no longer much of an issue.
* Advance downloading of assets that won’t be downloaded until needed, such as images that only appear upon `:hover` pseudo-states. Blinking wouldn't be seen.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### How would you approach fixing browser-specific styling issues?

* After identifying the issue and the offending browser, use a separate style sheet that only loads when that specific browser is being used. This technique requires server-side rendering though.
* Use libraries like Bootstrap that already handles these styling issues for you.
* Use `autoprefixer` to automatically add vendor prefixes to your code.
* Use Reset CSS or Normalize.css.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### What is CSS preprocessor and why to user one?

A **CSS preprocessor** is a program that lets you generate CSS from the preprocessor's own unique syntax. There are many CSS preprocessors to choose from, however most CSS preprocessors will add some features that don't exist in pure CSS, such as mixin, nesting selector, inheritance selector, and so on. These features make the CSS structure more readable and easier to maintain.

Here are a few of the most popular CSS preprocessors:

* SASS (SCSS)
* LESS
* Stylus
* PostCSS

###### Source

* https://developer.mozilla.org/en-US/docs/Glossary/CSS_preprocessor

[[↑] Back to top](#CSS)
### Have you ever worked with retina graphics? If so, when and what techniques did you use?

_Retina_ is just a marketing term to refer to high resolution screens with a pixel ratio bigger than 1. The key thing to know is that using a pixel ratio means these displays are emulating a lower resolution screen in order to show elements with the same size. Nowadays we consider all mobile devices _retina_ defacto displays.

Browsers by default render DOM elements according to the device resolution, except for images.

In order to have crisp, good-looking graphics that make the best of retina displays we need to use high resolution images whenever possible. However using always the highest resolution images will have an impact on performance as more bytes will need to be sent over the wire.

To overcome this problem, we can use responsive images, as specified in HTML5. It requires making available different resolution files of the same image to the browser and let it decide which image is best, using the html attribute `srcset` and optionally `sizes`, for instance:

```html
<div responsive-background-image>  
  <img src="/images/test-1600.jpg"
    sizes="
      (min-width: 768px) 50vw,
      (min-width: 1024px) 66vw,
      100vw"
    srcset="
      /images/test-400.jpg 400w,
      /images/test-800.jpg 800w,
      /images/test-1200.jpg 1200w">
</div>
```

It is important to note that browsers which don't support HTML5's `srcset` (i.e. IE11) will ignore it and use `src` instead. If we really need to support IE11 and we want to provide this feature for performance reasons, we can use a JavaScript polyfill, e.g. Picturefill (link in the references).

For icons, I would also opt to use SVGs and icon fonts where possible, as they render very crisply regardless of resolution.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### How is responsive design different from adaptive design?

Both *responsive* and *adaptive* design attempt to optimize the user experience across different devices, adjusting for different viewport sizes, resolutions, usage contexts, control mechanisms, and so on.

**Responsive design** works on the principle of flexibility — a single fluid website that can look good on any device. Responsive websites use *media queries*, *flexible grids*, and *responsive images* to create a user experience that flexes and changes based on a multitude of factors. Like a single ball growing or shrinking to fit through several different hoops.

**Adaptive design** is more like the modern definition of progressive enhancement. Instead of one flexible design, adaptive design detects the device and other features, and then provides the appropriate feature and layout based on a *predefined set of viewport sizes* and other characteristics. The site detects the type of device used, and delivers the pre-set layout for that device. Instead of a single ball going through several different-sized hoops, you’d have several different balls to use depending on the hoop size.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### How to create a zebra striped table with CSS?

To create a zebra-striped table, use the `nth-child()` selector and add a background-color to all even (or odd) table rows:
```css
tr:nth-child(even) {
    background-color: #f2f2f2
}
```

###### Source

* https://www.w3schools.com/howto/howto_css_table_zebra.asp

[[↑] Back to top](#CSS)
### What’s the difference between “resetting” and “normalizing” CSS? Which would you choose, and why?

* **Resetting** — is meant to strip all default browser styling on elements. For e.g. `margins`, `paddings`, `font-sizes` of all elements are reset to be the same. You will have to redeclare styling for common typographic elements.
* **Normalizing** — preserves useful default styles rather than “unstyling” everything. It also corrects bugs for common browser dependencies.

It's a good idea to choose resetting when you have very a customized or unconventional site design such that I need to do a lot of my own styling do not need any default styling to be preserved.


###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### How does CSS actually work (under the hood of browser)?

When a browser displays a document, it must combine the document's content with its style information. It processes the document in two stages:

* The browser converts *HTML* and *CSS* into the *DOM (Document Object Model)*. The DOM represents the document in the computer's memory. It combines the document's content with its style.
* The browser displays the contents of the DOM.

![](https://mdn.mozillademos.org/files/11781/rendering.svg)

###### Source

* https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/How_CSS_works

[[↑] Back to top](#CSS)
### Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.

The *CSS box model* is responsible for calculating:

* How much space a block-level element takes up.
* Whether or not borders and/or margins overlap, or collapse.
* A box’s dimensions

```css
div {
    width: 300px;
    border: 25px solid green;
    padding: 25px;
    margin: 25px;
}
```

The box model has the following rules:

* The dimensions of a block element are calculated by `width`, `height`, `padding`, `borders`, and `margins`.
* If no height is specified, a `block` element will be as high as the content it contains, plus padding (unless there are floats, for which see below).
* If no width is specified, a non-floated `block` element will expand to fit the width of its parent minus padding.
* The `height` of an element is calculated by the content's height.
* The `width` of an element is calculated by the content's width.
* By default, `paddings` and `borders` are not part of the width and height of an element.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### What is CSS selectors? Name some.

A CSS selector is the part of a CSS rule set that actually selects the content you want to style.

Consider some types of CSS selectors:
* **Universal selector**: `*`
* **Element type selector**: `ul`, `td`
* **ID Selector**: `#id`
* **Class selector**: `.box`
* **Descendant combinator**: `#id .box`. The .box element doesn’t have to be an immediate child of #id.
* **Child combinator**: `#id > .box`. Unlike the descendant combinator, there can’t be another element wrapping .box
* **General Sibling Combinator**: `~`
* **Adjacent Sibling Combinator**: `+`. The difference from general sibling combinaltor is that the targeted element must be an immediate sibling, not just a general sibling.
* **Attribute Selector**: `input[type="text"]`
* **Pseudo-class**: `a:hover`. A pseudo-class uses a colon character to identify a pseudo-state that an element might be in.
* **Pseudo-element**: `.container::before`. This selector inserts an imaginary element into the page, inside the targeted element, before its contents.




###### Source

* https://www.sitepoint.com/css-selectors/

[[↑] Back to top](#CSS)
### Explain the usage of "table-layout" property

The `table-layout` property defines the algorithm used to lay out table cells, rows, and columns.

```css
table-layout: auto|fixed|initial|inherit;
```

* **auto** - 	Browsers use an automatic table layout algorithm. The column width is set by the widest unbreakable content in the cells. The content will dictate the layout.
* **fixed** - 	The layout is fixed based on the first row. Set the width of those, and the rest of the table follows. If no widths are present on the first row, the column widths are divided equally across the table, regardless of content inside the cells.
* **initial** - Sets this property to its default value.
* **inherit** - Inherits this property from its parent element.



###### Source

* https://www.w3schools.com/cssref/pr_tab_table-layout.asp

[[↑] Back to top](#CSS)
### Describe pseudo-elements and discuss what they are used for.

A *CSS pseudo-element* is a keyword added to a selector that lets you style a specific part of the selected element(s). They can be used for decoration (`:first-line`, `:first-letter`) or adding elements to the markup (combined with `content: ...`) without having to modify the markup (`:before`, `:after`).

Example of usage:
* `:first-line` and `:first-letter` can be used to decorate text.
* Used in the `.clearfix` hack to add a zero-space element with `clear: both`.
* Triangular arrows in tooltips use `:before` and `:after`. Encourages separation of concerns because the triangle is considered part of styling and not really the DOM, but not really possible to draw a triangle with just CSS styles.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### What does Accessibility (a11y) mean?

**Accessibility (a11y)** is a measure of a computer system's accessibility is to all people, including those with disabilities or impairments. It concerns both software and hardware and how they are configured in order to enable a disabled or impaired person to use that computer system successfully.

Accessibility is also known as *assistive technology*.

###### Source

* https://www.techopedia.com/definition/10165/accessibility-a11y

[[↑] Back to top](#CSS)
### What are the advantages/disadvantages of using CSS preprocessors?

**Advantages:**

* CSS is made more maintainable.
* Easy to write nested selectors.
* Variables for consistent theming. Can share theme files across different projects.
* Mixins to generate repeated CSS.
* Splitting your code into multiple files. CSS files can be split up too but doing so will require a HTTP request to download each CSS file.

**Disadvantages:**

* Requires tools for preprocessing. Re-compilation time can be slow.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### What is a Grid System in CSS?

A grid system is a structure that allows for content to be stacked both vertically and horizontally in a consistent and easily manageable fashion. Grid systems include two key components: rows and columns.

Some Grid Systems:
* Simple Grid
* Pure
* Flexbox Grid
* Bootstrap
* Foundation

###### Source

* https://www.sitepoint.com/understanding-css-grid-systems/

[[↑] Back to top](#CSS)
### What's the difference between a `relative`, `fixed`, `absolute` and `static`ally positioned element?

A positioned element is an element whose computed `position` property is either `relative`, `absolute`, `fixed` or `sticky`.

* `static` - The default position; the element will flow into the page as it normally would. The `top`, `right`, `bottom`, `left` and `z-index` properties do not apply.
* `relative` - The element's position is adjusted relative to itself, without changing layout (and thus leaving a gap for the element where it would have been had it not been positioned).
* `absolute` - The element is removed from the flow of the page and positioned at a specified position relative to its closest positioned ancestor if any, or otherwise relative to the initial containing block. Absolutely positioned boxes can have margins, and they do not collapse with any other margins. These elements do not affect the position of other elements.
* `fixed` - The element is removed from the flow of the page and positioned at a specified position relative to the viewport and doesn't move when scrolled.
* `sticky` - Sticky positioning is a hybrid of relative and fixed positioning. The element is treated as `relative` positioned until it crosses a specified threshold, at which point it is treated as `fixed` positioned.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### Explain the purpose of clearing floats in CSS

The `clear` CSS property specifies whether an element can be next to floating elements that precede it or must be moved down (cleared) below them.

*Clearing floats* (or clearfixing) basically forces the containing element to expand to contain its child elements. It thus forces the subsequent elements to appear below it. 

###### Source

* https://www.sitepoint.com/clearing-floats-overview-different-clearfix-methods/

[[↑] Back to top](#CSS)
### How do you optimize your webpages for print?

* Create a stylesheet for print or use media queries.

```css
@media print {
  ...
}
```
* Add page breaks

```css
<style>
.page-break { 
  display: none;
  page-break-before: always; 
}
</style>
```
```html
Lorem ipsum dolor sit amet, consNullam aliquet. Aliquam ut diam...
<div class="page-break"></div>
Lorem ipsum dolor sit amet, consectetuer adipiscing elit....
```

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### Have you ever used a grid system, and if so, what do you prefer?

I like the `float`-based grid system because it still has the most browser support among the alternative existing systems (`flex`, `grid`). It has been used in for *Bootstrap* for years and has been proven to work.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### What are the different ways to visually hide content (and make it available only for screen readers)?

These techniques are related to accessibility (`a11y`).

* `visibility: hidden`. However the element is still in the flow of the page, and still takes up space.
* `width: 0; height: 0`. Make the element not take up any space on the screen at all, resulting in not showing it.
* `position; absolute; left: -99999px`. Position it outside of the screen.
* `text-indent: -9999px`. This only works on text within the block elements.
* `.sr-only` class for Bootstrap

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### Describe z-index and how a stacking context is formed

The `z-index` property in CSS controls the vertical stacking order of elements that overlap. `z-index` only effects elements that have a position value which is not `static`.

Without any `z-index` value, elements stack in the order that they appear in the DOM (the lowest one down at the same hierarchy level appears on top). Elements with non-static positioning (and their children) will always appear on top of elements with default static positioning, regardless of HTML hierarchy.

A *stacking context* is an element that contains a set of layers. A single default stacking context is created for every web page. The root of this context (the table) is the html element Or it can be a local stacking context, as created by specific properties and values. Within a local stacking context, the `z-index` values of its children are set relative to that element rather than to the document root.

<img src='https://cdn.tutsplus.com/webdesign/uploads/2013/11/stacking-contexts1.png' class='img-fluid'/>

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### What does * { box-sizing: border-box; } do? What are its advantages?

* By default, elements have `box-sizing: content-box` applied, and only the content size is being accounted for.
* `box-sizing: border-box` changes how the width and height of elements are being calculated, `border` and `padding` are also being included in the calculation.
* The `height` of an element is now calculated by the content's height + vertical `padding` + vertical `border` width.
* The `width` of an element is now calculated by the content's width + horizontal `padding` + horizontal `border` width.

Consider:

```css
div {
  width: 160px;
  height: 80px;
  padding: 20px;
  border: 8px solid red;
  background: yellow;
}

.content-box { 
  box-sizing: content-box; 
  /* Total width: 160px + (2 * 20px) + (2 * 8px) = 216px
     Total height: 80px + (2 * 20px) + (2 * 8px) = 136px
     Content box width: 160px
     Content box height: 80px */
}

.border-box { 
  box-sizing: border-box;
  /* Total width: 160px
     Total height: 80px
     Content box width: 160px - (2 * 20px) - (2 * 8px) = 104px
     Content box height: 80px - (2 * 20px) - (2 * 8px) = 24px */
}
```
```html
<div class="content-box">Content box</div>
<br>
<div class="border-box">Border box</div>
```
Result:

<img src='https://docs.google.com/uc?id=16N2TdSDvC_Pms70M6LvxcMiCHMSqe_dE' class='img-float'/>


###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### Can you explain the difference between coding a website to be responsive versus using a mobile-first strategy?

Note that these two 2 approaches are not exclusive.

Making a website responsive means the some elements will respond by adapting its size or other functionality according to the device's screen size, typically the viewport width, through CSS media queries, for example, making the font size smaller on smaller devices.

```css
@media (min-width: 601px) {
  .my-class {
    font-size: 24px;
  }
}
@media (max-width: 600px) {
  .my-class {
    font-size: 12px;
  }
}
```

A mobile-first strategy is also responsive, however it agrees we should default and define all the styles for mobile devices, and only add specific responsive rules to other devices later. Following the previous example:

```css
.my-class {
  font-size: 12px;
}

@media (min-width: 600px) {
  .my-class {
    font-size: 24px;
  }
}
```

A mobile-first strategy has 2 main advantages:

* It's more performant on mobile devices, since all the rules applied for them don't have to be validated against any media queries.
* It forces to write cleaner code in respect to responsive CSS rules.

###### Source

* https://codeburst.io/clearing-your-front-end-job-interview-css-95bdd82871f2

[[↑] Back to top](#CSS)
### Explain the basic rules of CSS Specificity

* ID selectors have a higher specificity than attribute selectors.
```css
/*wins*/
a#a-02 { background-image : url(n.gif); }
a[id="a-02"] { background-image : url(n.png); }
```
* Contextual selectors are more specific than a single element selector.
* The embedded style sheet is closer to the element to be styled. 
* The last rule defined overrides any previous, conflicting rules.
```css
p { color: red; background: yellow }
p { color: green } // wins
```
* A class selector beats any number of element selectors. 
```css
.introduction {} //wins
html body div div h2 p {}
```
* The universal selector has a specificity of `0, 0, 0, 0`.

###### Source

* https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/

[[↑] Back to top](#CSS)
### Is there any reason you'd want to use `translate()` instead of `absolute` positioning, or vice-versa? And why?

`translate()` is a value of CSS `transform`. Changing `transform` or `opacity` does not trigger browser reflow or repaint but does trigger compositions; whereas changing the absolute positioning triggers `reflow`. `transform` causes the browser to create a GPU layer for the element but changing absolute positioning properties uses the CPU. Hence `translate()` is more efficient and will result in shorter paint times for smoother animations.

When using `translate()`, the element still occupies its original space (sort of like `position: relative`), unlike in changing the absolute positioning.

###### Source

* https://www.paulirish.com/2012/why-moving-elements-with-translate-is-better-than-posabs-topleft/

[[↑] Back to top](#CSS)
### What the code fragment has the greater CSS specificity? 

The CSS specificity: 
* `A` is `0,0,0,1` (one element), 
* `B` is `0,1,0,1` (one ID reference point and one element), 
* `C` is `1,0,0,0` (since it is an inline styling).

Since
`0001 = 1 < 0101 = 101 < 1000`,

the third rule has a greater level of specificity, and therefore will be applied. If the third rule didn’t exist, the second rule would have been applied.

###### Source

* https://www.smashingmagazine.com/2007/07/css-specificity-things-you-should-know/

[[↑] Back to top](#CSS)
### What clearfix methods do you know? Provide some examples.

**Method 1. The Old School Way**

Insert an empty element that has the clear property declared on it at the bottom of the container of floated elements.

```css
.clear {
  clear: both;
}
```
```html
<div class="container">
  <div class="el-1">I'm floated...</div>
  <div class="el-2">I'm also floated...</div>
  <br class="clear">
</div>

<div class="main">
  Bravo, sirs and madams. I'm in the clear.
</div>
```
**Method 2: The Overflow Way**

Using the `overflow` property on our `.container`, we can actually force the container to expand to the height of the floated elements. 
```css
.container {
  overflow: hidden; /* can also be "auto" */
}
```
```html
<div class="container">
  <div class="el-1">I'm floated...</div>
  <div class="el-2">I'm also floated...</div>
</div>

<div class="main">
  Bravo, sirs and madams. I'm in the clear.
</div>
```
**Method 3: The “clearfix” Class**

The “clearfix” (which means fixing the clearing of floats) defines a `.clearfix` class in our stylesheet that we can apply to any float-containing element. This will force the container element to expand, pushing subsequent elements beneath it. It uses the CSS pseudo-elements `::before` and `::after`.
```css
.clearfix:before,
.clearfix:after {
  content: "";
  display: table;
}

.clearfix:after {
  clear: both;
}

.clearfix {
  zoom: 1; /* ie 6/7 */
}
```
```html
<div class="container clearfix">
  <div class="el-1">I'm floated...</div>
  <div class="el-2">I'm also floated...</div>
</div>

<div class="main">
  Bravo, sirs and madams. I'm in the clear.
</div>
```
**Method 4: The Future contain-floats Value**

The W3C specification has added a new value to the min-height property (and to other min/max properties), in order to help solve this problem. It looks like this:
```css
.container {
  min-height: contain-floats;
}
```
This basically will do the same thing as the clearfix or the overflow method, but with a single line of code.

###### Source

* https://www.sitepoint.com/clearing-floats-overview-different-clearfix-methods/

[[↑] Back to top](#CSS)
### How to style every element which has an adjacent item right before it?

Use **The Lobotomized Owl Selector**:
```css
* + * {
  margin-top: 1.5em;
}
```
The idea is that only elements that have a previous sibling inside a container get margin on top.

Another example:
```html
<div class="container">
  <div>Box 1</div>
  <div>Box 2
    <div>Sub-box 1</div>
    <div>Sub-box 2</div>
  </div>
  <div>Box 3</div>
</div>
```
Css:
```css
* + * {
  margin-top: 0.5em;
}

html, body {
  height: 100%;
}

body {
  font-family: "Roboto", san-serif;
  margin: 0;
  overflow: hidden;
}

.container {
	background: #ccc;
  min-height: 100%;
  padding: 2em;
}

.container div {
  background: #fff;
  border: 2px dashed #666;
  padding: 2em;
  width: auto;
}

.container div:nth-child(2) > div {
	background: #ccc;
}
```

###### Source

* https://css-tricks.com/spoooooky-css-selectors/

[[↑] Back to top](#CSS)
### Write down a selector that will match any links end in .zip, .ZIP, .Zip etc...

Use *case-insensitive attribute matching*, `i`. This is a new feature in CSS Selectors Level 4.

Consider:
```css
a[href$=".zip" i]:after {
  content: '↓'
}
```

###### Source

* https://css-tricks.com/spoooooky-css-selectors/

[[↑] Back to top](#CSS)
