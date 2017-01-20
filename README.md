# ionic-push-blank

```
  ## Install Ionic and Cordova globally
  $ npm install -g ionic cordova

  ## Add android platform to this project
  $ ionic platform add android
  
  ## Replace senderID
  $ cordova plugin add phonegap-plugin-push --variable SENDER_ID="XXXXXXX"
  
  ## Also replace your senderID in package.json and in config.xml
  
  ## Build an android-debug.apk
  $ ionic build android
```

Install it on your phone and check debug console. Your registrationId will be logged there.
