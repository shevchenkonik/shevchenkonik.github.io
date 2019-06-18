---
layout: post
title: "The difference between dependencies and devDependencies in Node Package Manager"
comments: false
description: "The article is about difference between devDependencies and dependencies"
keywords: "npm, devdependencies, dependencies"
---

## Specifying devDependencies (development) and dependencies (production)

When using [NPM](https://npmjs.com) (Node Package Manager) you should have seen file ``package.json``. In this file described information about package and you can see a list of all dependencies. Dependencies are divided into two types: dependencies and devDependencies.

### Two types of packages

The difference between these two types is dependencies are packages that needed for production environment while devDependencies are packages which are only needed for local environment & test's.

Dependencies (for runtime): [Axios](https://github.com/axios/axios), [Express](https://github.com/expressjs/express), [React](https://reactjs.org/), etc.

DevDependencies (for local environment & tests): [Babel](https://babeljs.io/), [Webpack](https://webpack.js.org/), [ESLint](https://eslint.org/), [Jest](https://jestjs.io/), etc.

To add dependencies to your project you need to do an ```npm install --save``` (shortcut: ```npm i -S```) and if you want to add devDependencies you can run the following command: ```npm install --save-dev``` (shortcut: ```npm i -D```). But if you install without flag, the package doesn't fit in ```packages.json```.