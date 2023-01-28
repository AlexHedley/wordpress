---
title: "Change Android SDK"
date: "2015-03-20"
categories: 
  - "android"
---

In Android Studio

Right click the App Folder

Open Module Settings (⌘↓)

Compile Sdk version (_x_)

Build Gradle

CompileSKDVersion

Doesn't change  other version.

Build errors for theme, was showing 21 since it was originally built with this.

Change the version here:

* * *

dependencies { compile 'com.android.support:appcompat-v7:19.0.0' }

* * *
