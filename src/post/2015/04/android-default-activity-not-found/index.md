---
title: "Android - Default Activity Not Found"
date: "2015-04-13"
categories: 
  - "android"
---

Check you AndroidManifest.xml has the correct name in the Activity

Another option:

```
File -> Invalidate Caches / Restart...
```

http://stackoverflow.com/questions/15825081/error-default-activity-not-found

I couldn't find this:

In Android Studio, right click on the project and choose **_Open Module Settings_**. Then go to the**_Sources_** tab in your module, find the **_src_** folder, right click on it and mark it as **_Sources_** (blue color).

http://stackoverflow.com/questions/18828654/default-activity-not-found-in-android-studio

Another error that went away with the above suggestions:

Gradle signing app with packageRelease “specified for property 'signingConfig.storeFile' does not exist”
