# Best Practice: PHP

## Description

[PHP](http://php.net) is an interpreted, multi-paradigm language used to create web applications. It’s also our standard backend language.

## Specific Standards

* Whenever possible, develop applications according to object-oriented principles, taking advantage of the object-oriented programming constructs in PHP.
* The principles, not the forms, of OOP are important. For example, “an object should avoid invoking methods of a member object returned by another method.” - [Law of Demeter](https://en.wikipedia.org/wiki/Law_of_Demeter)
* Use PHP 5.3 and up.
* New applications must follow [PSR-12](http://www.php-fig.org/psr/psr-12/), unless they use a framework or CMS that has its own coding standards (e.g., [Drupal](https://www.drupal.org/docs/develop/standards)).
* Commenting is strongly encouraged. If the code would be hard to explain verbally - comment it.
* “When in Rome”: follow the standards of the framework you’re working with.
* Use of any tools recommended by [phptherightway.com](http://www.phptherightway.com) is encouraged.
* Use Composer for including third-party code when possible.
* Don’t fix old things until we are working on them anyway. Then make them follow this standard.

## Rationale

We want to create code that is high quality (see “Good Enough for Everyone” best practice), and easy to maintain and work on collaboratively.

Code is communication.

Why OOP?  The power of OO comes mainly from inheritance and polymorphism.  When working on large applications with complex problems, it is necessary to abstract and encapsulate different families of functionality and data-structures. Objects can be passed around different branches of an application and manipulated without writing new functionality for each case.

Why have a coding standard? Mainly, clean code is necessary in a shared programming environment to efficiently test and review code, as well as work on shared files.

## Exceptions

3rd party code that is hard to touch, legacy projects that are near end of life.
