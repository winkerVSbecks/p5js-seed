p5js-seed
=========

You can use this project to quickly bootstrap your p5js project and supporting dev environment.

The seed contains a basic p5js application and is pre-configured to install the p5js framework and a bunch of development tools using bower and npm.


## Getting Started

To get you started you can simply clone the p5js-seed repository and install the dependencies:

```
git clone https://github.com/winkerVSbecks/p5js-seed.git
cd p5js-seed
```

## Install Dependencies

We have two kinds of dependencies in this project: dev tools and p5.js framework code. The tools help us preview the application.

We get the dev tools using npm and p5.js via bower.

npm is preconfigured to automatically run bower so, you can simply do:

```
npm install
```

After the above command finishes execution you should find that you have two new folders in your project:

- `node_modules` - contains the npm packages for the dev tools we need
- `bower_components` - contains the p5.js framework files

## Run the Application

We use [gulp](http://gulpjs.com) as a task-runner for this project. It's been pre-configured with a simple development web server and live-reload. The simplest way to start this server is:

```
gulp dev
```

Now browse to the app at http://localhost:3000

## Live Re-load
To enable live reload you will have to install the LiveReload plugin for your browser:

- [Chrome](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei?hl=en)
- [Safari](http://download.livereload.com/2.0.9/LiveReload-2.0.9.safariextz)
- [Firefox](https://addons.mozilla.org/en-US/firefox/addon/livereload/)


## Updating

You can update the tool dependencies by running:

```
npm update
```

This will find the latest versions that match the version ranges specified in the package.json file.

You can update the p5.js by running:

```
bower update
```

This will find the latest versions that match the version ranges specified in the bower.json file.
