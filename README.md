# IONIC tutorial: step1
This repository is part of the a presentation on developing mobile applications - demonstrating the design and process of building an hybrid mobile application.

The main target of the presentation is windows-oriented, so I will use windows command line and android development kit only (as IOS XCode does not work outside of OS-X)

This demonstration is based on the ionic tutorial found at:  [http://www.tutorialspoint.com/ionic](http://www.tutorialspoint.com/ionic)

## Todo
- Add link to presentation
- Add OS-X command line alternatives
- Add IOS support
- Add tests

## Prerequisites
You will need the following enviroments installed before we can start
* [node.js]: evented I/O for the backend (Use version 4, version 5 is currently not supported)
* [AndroidStudio]: Android development enviroment + development kit

## Optional
* [gitcmd]: GIT client
* [Brackets.io]: HTML & javascript editor (you can use whetever you feel comfortable with)
* [NVM windows]: Node.js version management for windows

## Step 1: Preparing the enviroment
Install prerequisites.

To install the IONIC and CORDOVA command lines, open command line and run the following:
```sh
npm install -g cordova ionic
```
This will use NPM (Node.js package manager) to install cordova and ionic as global components (need to do it only once - not per application)

## Step 2: Create a blank application
a. Create the blank application
```sh
C:\Projects\Demo\ionic-tutorial> ionic start ionic_sample_step1 blank
```
b. Switch to the application folder and generate an android project for it
```sh
C:\Projects\Demo\ionic-tutorial> cd ionic_sample_step1
C:\Projects\Demo\ionic-tutorial\ionic_sample_step1> ionic platform add android
```
c. Build the application
```sh
C:\Projects\Demo\ionic-tutorial\ionic_sample_step1> ionic build android
```
d. Run and test it
```sh
C:\Projects\Demo\ionic-tutorial\ionic_sample_step1> ionic run android
```
e. If you want to view it in a web browser
```sh
C:\Projects\Demo\ionic-tutorial\ionic_sample_step1> ionic serv
```

**Congratulations, you just built your hybrid app :-)**

## Step 3: Modify the application
Most of the changes will be done on next steps, for now we will just update some styling and show you how to edit the application.

First switch to the `www` folder. This is where you will mostly spend your time as it contains the application files.
```sh
cd www
```
and open the `index.html` file. 

Scroll down to the `ion-header-bar`element.
* change its style from 'bar-stable' to 'bar-positive'. This will change the header background to light blue.
* change the header title from 'Ionic Blank Starter' to 'My Tasks'

And just because I hate undescriptive names, change the angular app name (the `ng-app` attribute in the `body` element from "starter" to "MyTasks"
So the new header will look like this:
```
   <body ng-app="MyTasks">
    <ion-pane>
      <ion-header-bar class="bar-positive">
        <h1 class="title">My Tasks</h1>
      </ion-header-bar>
      <ion-content>
      </ion-content>
    </ion-pane>
  </body>
```
And since we changed the application name in the HTML file, we will also need to modify the main module name of angular application file.

To do this, open the `app.js` file under the `js` folder (this is the angular main module) and change change the angular module name on top from 'starter' to 'MyTasks'.
```
angular.module('MyTasks', ['ionic'])
```
Now run the application to test it


### Version

0.1.0

###License

MIT

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [gitcmd]: <https://git-scm.com/downloads>
   [node.js]: <http://nodejs.org>
   [AndroidStudio]: <http://developer.android.com/sdk/index.html>
   [Brackets.io]: <http://brackets.io/>
   [NVM windows]: <https://github.com/coreybutler/nvm-windows>