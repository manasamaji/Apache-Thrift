# Thrift tutorial with Angular and Webpack

This repository implements the [Apache Thrift tutorial](https://thrift.apache.org/tutorial/js) using Angular 2 and Webpack.

## Prerequisites

Node.js and npm are essential to Angular development. 
    
<a href="https://docs.npmjs.com/getting-started/installing-node" target="_blank" title="Installing Node.js and updating npm">
Get it now</a> if it's not already installed on your machine.
 
**Verify that you are running at least node `v4.x.x` and npm `3.x.x`**
by running `node -v` and `npm -v` in a terminal/console window.
Older versions produce errors.

## Clone this repository

```bash
git clone https://github.com/osechet/angular-thrift
cd angular-thrift
```

## Install npm packages

> See npm version notes above

Install the npm packages described in the `package.json` and verify that it works:

```bash
npm install
npm start
```

The `npm start` command first compiles the application, 
then uses webpack to bundle it and run a development web server.
Webpack watches for file changes.

Shut it down manually with `Ctrl-C`.

### Apache Thrift server

To work, the application needs a Thrift HTTP server using the JSON protocol. You can use the one provided by the Javascript tutorial: 
```
cd /path/to/thrift/tutorial/js
make tutorialserver
```

### Run with Electron

To work with Electron in development, call:

```bash
npm run start.desktop
```

The `npm run start.desktop` command first compiles the application, 
then uses webpack to bundle it and starts Electron to load the application.
Webpack watches for file changes and reloads Electron when needed.

