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
6. _Optional_: Use the `home-dir` template by creating a series of symlinks:

```bash
$ cd
$ ln -s ~/Documents/developer-essentials/home-dir .home-dir
$ ln -s ~/.home-dir/bin bin
$ ln -s ~/.home-dir/sh/aliases ~/.bash_aliases
```

## Installing Other Software

Since we do mostly software development, let's get setup with a few essential tools.

### NodeJS

NodeJS is a server-side Javascript engine that has become popular for web development in recent years.
For a developer workstation, I recommend installing NodeJS by doing the following:

 1. Download the most recent [LTS release of NodeJS](https://nodejs.org/en/) into your `~/bin/` directory.
 2. From the command-line `cd` into your `bin` directory & extract the archive: `tar -xvf <filename>.tgz`. This will create a new folder named something like `node-v8.9.1-linux-x64`.
 3. Create a symlink to this folder to make future updates easier: `ln -s node-v8.9.1-linux-x64 nodejs`
 4. Create symlinks to the executable commands `ln -s nodejs/bin/node`, `ln -s nodejs/bin/npm`

 Now you can execute the `node` and `npm` commands from anywhere (because your homedir's `bin` directory is part of your PATH environment variable).

```bash
$ node --version
v8.9.1

$ npm --version
5.5.1
```

### PHP

PHP is an older, tried-and-true scripting language commonly used for web development.
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

1. Run `npm install && npm run serve`
2. Visit http://localhost:3000 in your web browser

(If that doesn't make sense to you, don't worry, just start with the README.)

## Contribute To This Project

This project is probably incomplete.
Help make it better by submitting requests for new or missing information and resources by creating an issue.
Or take it a step further by opening both issue and a Pull Request that resolves the issue.
