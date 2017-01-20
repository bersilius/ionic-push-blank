# ionic-push-blank

This is a template Ionic application for using [phonegap-plugin-push](https://github.com/phonegap/phonegap-plugin-push).
Follow the instruction below on how to build an Android (Ionic) application.

Note, that in order to use this application you must have JAVA and Android SDK installed.
TODO: Create walkthrough for JAVA and Android SDK install and usage

```
  ## Install Ionic and Cordova globally
  $ npm install -g ionic cordova
  
  ## Run npm install first time
  $ npm install

  ## Add android platform to this project
  $ ionic platform add android
  
  ## Replace senderID
  $ cordova plugin add phonegap-plugin-push --variable SENDER_ID="XXXXXXX"
  
  ## Also replace your senderID in package.json, www/js/app.js and in config.xml
  
  ## Build an android-debug.apk
  $ ionic build android
```

Install it on your device and check debug console. Your registrationId will be logged there.
