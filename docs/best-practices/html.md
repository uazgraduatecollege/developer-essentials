# Best Practice: HTML

## Description
HTML is the standard markup language used to create web pages. It is the foundational language of the web, and its primary role is to describe the semantic structure of content displayed on a web page. 

## Specific Standards

### Separate presentation from markup

HTML tags should be used for structuring content, and should generally not be used for presentation (that’s what CSS is for). 

Examples of presentational HTML (which should be avoided):

* `<font>` - Font properties should be defined in CSS. 
* `<br />` - Proper use of block level HTML elements or `display: block;` in CSS should be used on inline elements to break content vertically.
* `<table>` for layout

### Use semantic HTML(5)

* Whenever possible, use an HTML tag that represents the content it contains.
* HTML5 introduced many new semantic elements, which should be used whenever possible.
* HTML5 Doctor is a great resource for figuring out which element is best to use.

### Follow basic HTML syntax & validation rules

This covers things like:

* All tags are properly closed: 
  - Correct: `<li>list item</li>`
  - Incorrect: `<li> list item`
* Tags are written in lower case:
  - correct: `<article>…</article>`
  - incorrect: `<ARTICLE></ARTICLE>`
* Attribute values are wrapped in quotes
  - correct: `<div class=“column”>…</div>`
  - incorrect: `<div class=column>…</div>`
  
More information:

* http://validator.w3.org/
* http://validator.w3.org/docs/why.html
* http://blog.codinghorror.com/html-validation-does-it-matter/

### Follow basic code quality standards

Coding standards is a larger subject that will be likely be addressed in the future in a separate UX-Dev best practice, but the basics should still be followed:

* Consistent code indentation
* Use alt attributes for `<img>` elements
* Don’t fix old things until we are working on them anyway. Then make them follow this standard.
* Don’t echo HTML. Just write it if possible.

## Rationale
We want to create code that is high quality (see “Good Enough for Everyone” best practice), and that easy to maintain and work on collaboratively.

Code is communication.

Unlike scripting languages like JavaScript where a single missing character is likely to break something, HTML errors are generally well tolerated by web browsers. This fault tolerance is good for users in that a web page’s content will generally remain accessible even with poorly coded HTML. However, this also means that errors and poorly coded HTML can go unnoticed. 

While it may not be obvious to users, poorly coded HTML can cause major problems for developers, especially in a team setting where others will be working with your code.

## Exceptions
3rd party code that is hard to touch, legacy projects that are near end of life.

## History
* Approved by UX-Dev on July 3, 2014
* Open sourced on July 17, 2017

