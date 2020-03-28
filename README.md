# Landing page
Based on [Web starter kit](https://github.com/justcoded/web-starter-kit/releases)

## Install

Init your project using [jcn](https://github.com/justcoded/npm-jcn) or directly [download WSK](https://github.com/justcoded/web-starter-kit/releases/latest) and run `$ npm install --global gulp && npm install` in that directory to get started.


To take advantage of WSK you need to:

1. Download the code.
2. Install all necessary dependencies if you don't already have them.
3. Modify the application as you wish.
4. Make the production of your code.

This starter wasn't tested on Linux. If you want to use it on Ubuntu 17 type these commands in a command terminal:
```sh
$ sudo snap install node --classic --channel 6/stable
```
```sh
$ npm install gulpjs/gulp-cli -g
```

## Prerequisites

### [Node.js](https://nodejs.org)

Bring up a terminal and type `node --version`.
Node should respond with a version at or above 8.0.x.
If you need to install Node, go to [nodejs.org](https://nodejs.org) and click on the big green Install button.

### [Gulp](http://gulpjs.com)

Bring up a terminal and type `gulp --version`.
If Gulp is installed it should return a version number at or above 4.0.x.
If you need to install/upgrade Gulp, open up a terminal and type in the following:

```sh
$ npm install --global gulp
```

*This will install Gulp globally. Depending on your user account, you may need to [configure your system](https://github.com/sindresorhus/guides/blob/master/npm-global-without-sudo.md) to install packages globally without administrative privileges.*


### Local dependencies

Next, install the local dependencies WSK requires:

```sh
$ npm install
```

That's it! You should now have everything needed to use the WSK.  
You may also want to get used to some of the [commands](#commands) available.


## Commands

There are few commands available to help you build and test sites:

### Development mode

Watch For Changes & Automatically Refresh Across Devices

```sh
$ gulp
```

`gulp` task creates the `assets` folder in the root of the project.
This includes linting as well as image, script, stylesheet and HTML optimization.
Also, a [browsersync](https://browsersync.io/) script will be automatically generated, which will take care of precaching your sites resources.


### Production mode

Serve the Fully Built & Optimized Site

```sh
$ gulp build
```

`gulp build` task creates the `production` folder in the root of the project with **minifying** files from `assets`. It will help you to create clear instances of code for the **production** or **further implementation**.


### Deploy

```sh
$ gulp deploy
```

### Linter - only for JS

```sh
$ gulp lint-js
```