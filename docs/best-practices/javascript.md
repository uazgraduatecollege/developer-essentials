# Best Practice: JavaScript

JavaScript is an interpreted, functional programming language. It was given the unfortunate name “JavaScript” as a ploy to make it more popular in the ‘90’s when the browser wars were starting to escalate. It does not use any Java functionality. We will alternately refer to its standardized name, “ECMAscript”. JavaScript is used mostly as an asynchronous language *on the client side*. It is, however, gaining popularity as a server-side, object oriented language (see Node.js). For our purposes, these best practices will apply to client-side usage. Also, take a look at http://jstherightway.org/.

## Specific Standards

* Avoid globally declared variables like the plague. Use of a [module pattern ](http://christianheilmann.com/2007/08/22/again-with-the-module-pattern-reveal-something-to-the-world/) or [IIFE pattern](http://benalman.com/news/2010/11/immediately-invoked-function-expression/) will simplify code and encapsulate variables.
* If a block of code isn’t easily readable, comment it with C comment syntax: `/* .. */`.
* Use notation shortcuts when possible, but don’t obfuscate the rationale behind the code.
* Cache variables whenever possible to avoid over-taxing resources. This is best for optimizing loops.
* Don’t append the DOM in a loop.
* Use exception handling for run-time errors. Remember, syntax errors will stop page loading, but run-time errors may be silent. Let’s do our part to catch them!
* We want to “use strict” (directive) with our scopes, either defined by function, or globally. This helps prevent errors.
* Avoid using browser specific code (like “sniffers”). Many other JS libraries have up-to-date code to handle old, unsupported browsers. See jQuery and modernizr below.
* Styles should be kept in the CSS.

## Frameworks and libraries we or our vendors use:

* http://jquery.com
* https://modernizr.com
* https://angularjs.org
* http://backbonejs.org
* http://underscorejs.org
* http://parsleyjs.org and http://garlicjs.org
* https://nodejs.org/en/
* http://expressjs.com

## Rationale
We want to create code that is high quality (see “Good Enough for Everyone” best practice), and easy to maintain and work on collaboratively.

Why use JS/ECMA? It’s almost impossible to *not* use ECMAScript on a web application, anymore. JS was designed to handle user events and make asynchronous transactions easy.

Code is poetry, too.

## Exceptions

3rd party code that is hard to touch, legacy projects that are near end of life.
