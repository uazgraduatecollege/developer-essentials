# Best Practice: Developer Documentation

## Overview

Developer-facing documentation is essential for communicating information about how to begin development on a new project, or how a project is designed to be configured and used.
This best practice is designed to be a guide for repository-level documentation, i.e., the documentation which would live on the filesystem in the project's source control repository.


## Rationale

Documentation preserves developer knowledge and reduces waste.
It gives a developer a place to explain how to use their project to other developers and it helps new developers get up and running quickly.
In a well-documented project, you can stand on the shoulders of the other developers.

## Specifics

### Git Repository Contents

#### README.md

There must be a README.md file in the project's root directory.
See this repository's [examples/README.md](https://github.com/uazgraduatecollege/developer-essentials/blob/master/examples/README.md) file for suggested content.

#### LICENSE

Add a `LICENSE` file.
Most Grad IT projects will belong to ABOR so use the following (be sure to update the year as needed):

```txt
Copyright (c) 2019 The Arizona Board of Regents on behalf of the University of Arizona - All Rights Reserved.
```

#### Editorconfig

Add an `.editorconfig` file. This will help standardize your coding style across editors and environments.
In most cases, you can use this repository's [examples/.editorconfig](https://github.com/uazgraduatecollege/developer-essentials/blob/master/examples/.editorconfig) file.

Visit [Editorconfig](https://editorconfig.org/) for a more complete introduction to what `.editconfig` can do for you.

### Comments

Use comments in your code.
When possible, refer to your language-specific best practices (like PHPdoc, JavaDoc, for example).
Make it easy for the next person (which might be you) to understand what's going on.

### Issues

Whichever git repository host is being used, we typically will use an issue tracker for documenting bugs and enhancement features.
In many cases, it will be helpful to describe the issue using a template, and in fact GitHub and GitLab can even make use of issue templates that are included in the repository
Issues can be adapted from the templates in whatever way is suitable - eg. our enhancement feature template includes a section for proposed SQL changes, which can be removed entirely if not relevent.

Current templates are in this repository's `examples` folder:

`examples`
  - .github\ISSUE_TEMPLATES
    - [bug_report.md](https://github.com/uazgraduatecollege/developer-essentials/blob/master/examples/.github/ISSUE_TEMPLATES/bug_report.md)
    - [feature_request.md](https://github.com/uazgraduatecollege/developer-essentials/blob/master/examples/.github/ISSUE_TEMPLATES/feature_request.md)
  - .gitlab
    - [Bug.md](https://github.com/uazgraduatecollege/developer-essentials/blob/master/examples/.gitlab/Bug.md)
    - [Enhancement.md](https://github.com/uazgraduatecollege/developer-essentials/blob/master/examples/.gitlab/Enhancement.md)

For projects hosted primarily in BitBucket, any of these templates may be copied and pasted - or merely used as a guideline - when creating new issues.

### Additional documentation

Additional documentation should be located in `./docs/`.

### Features

We're starting to use Gherkin for describing user-facing functionality, and have learning about best practices from a couple of resources:

 - [BDD 101: Writing Good Gherkin](https://automationpanda.com/2017/01/30/bdd-101-writing-good-gherkin/)
 - [Behat: Writing Features](http://docs.behat.org/en/v2.5/guides/1.gherkin.html)

Gherkin features should be in the project's `./docs/features/` directory, and may be further sorted into subdirectories named for user Personas.
Eg.:
 - `./docs/features/Applicants/`
 - `./docs/features/Faculty/`

Feature files should use a file extensin of `.feature` and should describe exactly one Feature.

### Markdown

[Markdown](http://commonmark.org) is the preferred format for all other documentation.

[Docsify](https://docsify.js.org/#/) is a nice static site generator for documentation written in Markdown.
See this repository's `docs/index.html` for a usage example.


## Exceptions

Features or other documentation may be kept in a separate repository, especially in the case of projects that span multiple repositories.
In such cases, the location of the documentation should be referenced in the README.md.


