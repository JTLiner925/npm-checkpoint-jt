to install nvm 
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash

To see a list of all Node versions that are available, run:
$ nvm ls-remote

nvm use 10.13.2

Create React App create-react-app 
https://github.com/facebook/create-react-app
is a tool developed by Facebook to quickly bootstrap a new React application complete with all the configurations that you may need for making awesome applications. It is a stadium rock concert in a box.

The environment created contains a large number of features. From the official docs, these are:

-React, JSX, ES6, and Flow syntax support
-language extras beyond ES6 like the object spread operator
-autoprefixed CSS, so you don’t need -webkit- or other prefixes
-a fast interactive unit test runner with built-in support for coverage reporting
-a live development server that warns about common mistakes
-a build script to bundle JS, CSS, and images for production, with hashes and sourcemaps
-an offline-first service worker and a web app manifest, meeting all the Progressive Web App criteria
-hassle-free updates for the above tools with a single 

To start a new app execute the create-react-app command with the name of the application that you would like to build. For instance, to create an application named my-first-react-app use the command:

$ npx create-react-app my-first-react-app

Notice the use of npx so Create React App does not have to be installed locally.

open folder in editor
cd my-first-react-app

Start
$ npm start

execute this script. It runs the app in development mode, which means that if you edit a file the page will automatically reload in the browser.

Test
To run the tests on the app use the command:

$ npm test

Build
To prepare your app for production deployment run the command:

$ npm run build

Eject (...but really, don't do this one!)
Sometimes you may wish to tweak the scripts and your build environment in some unique way. In that case, you can eject. That removes the single dependency and copies everything directly into your project. However, this is a one-way process and once ejected you cannot go back to the single dependency for that project.

npm
As described above, npm is a tool to help you make use of the many open sourced Node packages that are available for free. 
The Node Package Manager (npm) is a tool for helping you obtain and manage the Node packages that you need. 

Official site: https://www.npmjs.com/
The features of the site we will look at are:

search for packages - autofill feature, learn about 
different packages and helpful ways to use specific packages

install packages locally
When you use a package as a building block in your own application we say that package is a dependency for your application.The way this is done is via the configuration file named package.json at the root of your application.Also, the code for the package is downloaded and stored in a directory named node_modules at the root of your application. 

say we need to print some dates in various formats or even do some date arithmetic. We can try writing the code to format a date ourselves which is very possible but can be very complex at times. For instance, what is the date 7 days from now? Can you write some code that will always give the right answer no matter what date you start with? Suppose it's a leap year and the start date is February 25?
The excellent 
moment 
library is a JavaScript library for parsing, manipulating and formatting dates.
To install the package use the npm install command. This command requires the name of the package. It downloads the package into a directory named node_modules.
$ npm install moment

After you run the command, open the package.json file and observe the property dependencies with the package listed.

do not need to edit Package-lock.json.
import statements are used to make various JavaScript modules available for use in this file.
import React from 'react';
import logo from './logo.svg';
import './App.css';

after downloading a package, you need to access it...do that by:
import moment from 'moment';

//to look at formatting 
https://momentjs.com/docs/#/displaying/


remove a package
Occasionally it becomes necessary to remove packages that have been installed previously. To remove a package use the npm uninstall command.
$ npm uninstall mathjs
When you uninstall a package, if you try to run your code again you will get an error. Need to remove the import and correlated info.

list installed packages
To see a list of packages that you have installed in your project use the 
npm ls command. 

NPM Scripts is a very powerful feature that makes it possible to automate just about any task.
i.e.  go to the scripts: in your package.json file and input: 
"my_script": "echo 'This is my npm script!' "

This is a script named "my_script" and the command associated with it is the echo command which simply prints the text on the screen. 
npm run my_script

To learn more on shell scripts
https://linuxconfig.org/bash-scripting-tutorial-for-beginners