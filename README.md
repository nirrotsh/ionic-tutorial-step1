# IONIC tutorial: step1
This repository is part of the a presentation on developing mobile applications - demonstrating the design and process of building an hybrid mobile application.

The main target of the presentation is windows-oriented, so I will use windows command line and android development kit only (as IOS XCode does not work outside of OS-X)

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

**Congrattiulations, you just built your hybrid app :-)**

*Now, lets add some content into it*

### Version
0.1.0

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [@thomasfuchs]: <http://twitter.com/thomasfuchs>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [marked]: <https://github.com/chjj/marked>
   [Ace Editor]: <http://ace.ajax.org>
   
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [keymaster.js]: <https://github.com/madrobby/keymaster>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]:  <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>

   [gitcmd]: <https://git-scm.com/downloads>
   [node.js]: <http://nodejs.org>
   [AndroidStudio]: <http://developer.android.com/sdk/index.html>
   [Brackets.io]: <http://brackets.io/>
   [NVM windows]: <https://github.com/coreybutler/nvm-windows>