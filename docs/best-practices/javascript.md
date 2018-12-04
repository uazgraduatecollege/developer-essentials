# Best Practice: JavaScript

JavaScript is an interpreted, functional programming language. It was given the unfortunate name _JavaScript_ as a ploy to make it more popular in the 90s when the browser wars were starting to escalate. It does not use any Java functionality. We will alternately refer to it as _JS_ or by its standardized name, _ECMAscript_. We used JavaScript for both client- and server-side development.

## Specific Standards

* We are embracing [StandardJS](https://standardjs.com/) as our preferred style.
* We prefer the use of `let` and `const` instead of `var`, [whenever possible](https://medium.com/podiihq/javascript-variables-should-you-use-let-var-or-const-394f7645c88f).
* If a block of code isn’t easily readable, comment it with C comment syntax: `/* .. */`.
* Use exception handling for run-time errors. Remember, syntax errors will stop page loading, but run-time errors may be silent. Let’s do our part to catch them!
* We want to `use strict` (directive) with our scopes, either defined by function, or globally. This helps prevent errors.
* Avoid using browser specific code (like _sniffers_). Many JS libraries have up-to-date code to handle old, unsupported browsers. See jQuery and modernizr below.
* Styles should be kept in the CSS.

## Frameworks and Libraries We Use or Are Beginning to Use

* [jQuery](https://jquery.com/)
* [Modernizr](https://modernizr.com/)
* [NodeJS](https://nodejs.org/)
* [Express](https://expressjs.com/)
* [Vue.js](https://vuejs.org/)
* [GatsbyJS](https://www.gatsbyjs.org/)

## Rationale
We want to create code that is high quality (see “Good Enough for Everyone” best practice), and easy to maintain and work on collaboratively.

Why use JS/ECMA? It’s almost impossible to *not* use ECMAScript on a web application, anymore. JS was designed to handle user events and make asynchronous transactions easy.

Code is poetry, too.

## Exceptions

3rd party code that is hard to touch, legacy projects that are near end of life.
