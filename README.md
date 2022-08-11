# Essentials For New Developers At The Graduate College

## About

This project is meant to help both new team members and those new to Linux to understand & work within the Web Team desktop environment.

## Getting Started

1. Create a BitBucket account and/or a GitHub account (please use your UA email address)
2. Let an administrator know your account username(s) so we can add you to the team accounts
3. Fork this repository
4. Clone it to your desktop computer:
  - `cd Documents`
  - `git clone git@github.com:yourusername/developer-essentials.git`
5. Read the docs
6. _Optional_: Use the `home-dir` template by creating a series of symlinks:

```bash
$ cd
$ ln -s ~/Documents/developer-essentials/home-dir .home-dir
$ ln -s ~/.home-dir/bin bin
$ ln -s ~/.home-dir/sh/aliases ~/.bash_aliases
```

## Installing Other Software

Since we do mostly software development, let's get setup with a few essential tools.

### Node.JS

Node.JS is a popular server-side Javascript engine.
For a developer workstation, we recommend installing Node.JS using the Node Version Manager (NVM).

1. Follow the instructions to [install NVM](https://github.com/nvm-sh/nvm#installing-and-updating).  
   You can verify your installation at the command-line: `$ nvm --version`

2. Use nvm to install and use the current Long-Term Service release of Node JS and npm:  
   `$ nvm install --lts && nvm use --lts`

You should now be able to execute the `node` and `npm` commands from anywhere:

```bash
$ node --version
v16.16.0

$ npm --version
8.11.0
```

### PHP

PHP is a tried-and-true scripting language commonly used for web development.
PHP can easily be installed from Ubuntu's package manager:

`sudo apt update && sudo apt install php-cli`

Now you can execute the `php` command. Eg.:

```bash
$ php --version
PHP 7.0.28-0ubuntu0.16.04.1 (cli) ( NTS )
Copyright (c) 1997-2017 The PHP Group
Zend Engine v3.0.0, Copyright (c) 1998-2017 Zend Technologies
    with Zend OPcache v7.0.28-0ubuntu0.16.04.1, Copyright (c) 1999-2017, by Zend Technologies
```

### Docker

TBD

## Read The Docs

Start with the [README](docs/README.md) file in the docs directory

You can even browse these docs with [Docsify](https://docsify.js.org/#/):

1. Install docsify: `npm install --global docsify-cli`
1. Run `npm run serve`
2. Visit http://localhost:3000 in your web browser (or whichever URL is reported)

(If that doesn't make sense to you, don't worry, just start with the README.)

## Contribute To This Project

This project is probably incomplete.
Help make it better by submitting requests for new or missing information and resources by creating an issue.
Or take it a step further by opening both issue and a Pull Request that resolves the issue.
