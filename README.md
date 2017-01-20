# ionic-push-blank

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
