# Essentials For New Developers At The Graduate College

## About

This project is meant to help both new team members and those new to Linux to understand & work within the Web Team desktop environment.

## Getting Started

1. Create a BitBucket account (please use your UA email address)
2. Let an administrator know your account username so we can add you to the team
3. Fork this repository
4. Clone it to your desktop computer:
  - `cd Documents`
  - `git clone git@bitbucket.org:yourusername/developer-essentials.git`
5. Read the docs
6. _Optional_: Use the `home-dir` template by creating a series of symlinks

```bash
$ cd
$ ln -s ~/Documents/developer-essentials/home-dir .home-dir
$ ln -s ~/.home-dir/bin bin
$ ln -s ~/.home-dir/sh/aliases ~/.bash_aliases
```

## Read The Docs

Start with the [README](docs/README.md) file in the docs directory

You can even browse these docs with [Docsify](https://docsify.js.org/#/):

1. Run `npm install && npm run serve`
2. Visit http://localhost:3000 in your web browser

(If that doesn't make sense to you, don't worry, just start with the README.)

## Contribute To This Project

This project is probably incomplete.
Help make it better by submitting requests for new or missing information and resources by creating an issue.
Or take it a step further by opening both issue and a Pull Request that resolves the issue.
