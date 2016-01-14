# Drupal Dev Days Milan 2016 ionic mobile test app
## Version: 0.1
Contibutors: Italo Mairo (www.italomairo.com)

## Perform Global requirements (For more info: http://ionicframework.com/docs/guide/installation.html)

### First, install Node.js 4 (Node 5 does not work at the moment!): https://nodejs.org/en/

## Then you need to install cordova and ionic as global requirements 

## Install cordova
$ sudo npm install -g cordova

## Install Ionic
$ sudo npm install -g ionic

### Set up, mount it and test in your local environment this ionic mobile test app (named: "ddd-ionic")

### Position yourself in the ionic-app folder and run the followings commands, it means from the website root:

$ cd ionic-app

$ npm install

$ bower install

## enable the iOS and Android platforms
$ ionic platform add ios
$ ionic platform add android

### Configure the link with your specific drupal instance (local host url) in the file: ionic-app/www/js/config.js

### Set to True the Drupal 8 permission RESTful Web Services => "Access GET on Content resource" to the Anonymous User (otherwise the app won't be able to expose the single Content page

### Test it out, as web app, just going here in your local server: http://path/to/ddd_website/ionic-app/www

### Test it out, as mobile app (substitute ios for android to build for Android instead) running the following commands:
$ ionic build ios
$ ionic emulate ios