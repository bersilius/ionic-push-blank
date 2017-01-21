# ionic-push-blank

This is a template Ionic application for using [phonegap-plugin-push](https://github.com/phonegap/phonegap-plugin-push).
Follow the instruction below on how to build an Android (Ionic) application.

## Important notices
This template has a (by default) generated package name: 'com.ionicframework.ionicpushblank132692'.
Although this code is only for experimenting, it does not mean that it is not stable.

This is not a template for further "production" development. You can find documentation links at the bottom to find out how to do this from scratch.

There are some steps while you create your own final .apk where you have to use some unique IDs. Those are only your secret. And they are mandatory variables for building your test app. These are like: FCM server API key, senderID. Also when you publish your app in a store (Google Play) the package name has to be unique.

In order to use this application you must have JAVA and Android SDK installed.
TODO: Create walkthrough for JAVA and Android SDK install and usage

So this template is meant to help set up everything, with several commands, changing some IDs in the code and configuring the 3rd party services. To have a quite "quick" start with the least effort. 

## How to set up and use this app

Firebase
// TODO: extend service examples
- create a new account or use a Google account to log in
- create a new project
- if you see your project view, on the top left you find a gear icon. Click to open project settings!
- choose the CLOUD MESSAGING tab, there you will find your Sender ID
- Sender ID is needed for next steps

```
  ## Install Ionic and Cordova globally
  $ npm install -g ionic cordova
  
  ## Run npm install first time
  $ npm install

  ## Add android platform to this project
  $ ionic platform add android
  
  ## Replace senderID
  $ cordova plugin add phonegap-plugin-push --variable SENDER_ID="XXXXXXX"
  
  ## Replace your senderID in package.json, www/js/app.js and in config.xml
  
  ## Build an android-debug.apk
  $ ionic build android
```

Install it on your device and open Chrome inspect debug console (chrome://inspect/#devices). Your registrationId will be logged there.
Use this registrationId to identify a device endpoint for push notification services.

Head to Firebase console again:
- add a new Android application (package name: com.ionicframework.ionicpushblank132692)
- click on "Notification" on the left pane
- click on "New Message"
- add the "Message text"
- on the "Target" selection, select "Single device" radio-button
- use your registrationId as "FCM registration token"
- edit other optional field
- click send "Message button"
- check your app debug console. If your app is in the foreground, without the sound enabled options the message will only appear in the debug console if you use Chrome inspector (chrome://inspect/#devices) // TODO: upgrade  template app to log message on app's default view

# References:

- [Create an Ionic app](https://ionicframework.com/getting-started/)
- [Install, setup and use phonegap/phonegap-plugin-push](https://github.com/phonegap/phonegap-plugin-push)
- [Firebase docs](https://firebase.google.com/docs/)
- see above steps in this README for Firebase project setup related steps
