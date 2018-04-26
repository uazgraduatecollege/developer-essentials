# Best Practice: Developer Documentation

## Description

Developer-facing documentation is essential for communicating information about how to begin development on a new project, or how a project is designed to be configured and used. This best practice is designed to be a guide for repository-level documentation, i.e., the documentation which would live on the filesystem in the project's source control repository.

## Specific Standards

### README

There must be a README in the project's root directory. See this repository's `examples/README.md` file for suggested content.

### LICENSE

Add a `LICENSE` file. Until we have a licensing best practice, here's the default, closed-source license.
More open licensing (i.e. MIT) is permitted.

```txt
Copyright (C) The Arizona Board of Regents on Behalf of the University of Arizona - All Rights Reserved
```

### Editorconfig

Add an `.editorconfig` file. In most cases, you can use the `examples/.editorconfig` file or [this snippet](https://bitbucket.org/snippets/uazgraduatecollege/Le4Mgo/editorconfig)

### Comments

Use comments in your code. When possible, refer to your language-specific best practices (like PHPdoc, JavaDoc, for example).
Make it easy for the next person (which might be you) to understand what's going on.

Generally helpful tips: https://msdn.microsoft.com/en-us/library/aa260844(v=vs.60).aspx#cfr_comments

### Markdown

[Markdown](http://commonmark.org) is the preferred format for documentation.

### Additional documentation

Additional documentation should be located in `./docs`.

[Docsify](https://docsify.js.org/#/) is a nice static site generator for documentation.

See this repository's `docs/index.html` for a usage example.

## Rationale

Documentation preserves developer knowledge and reduces waste. It gives a developers a place to explain how to use their project to other developers and it helps new developers get up and running quickly. In a well-documented project, you can stand on the shoulders of the other developers.

## Exceptions

In general, more documentation is better than less. There probably aren't many exceptions to this rule.