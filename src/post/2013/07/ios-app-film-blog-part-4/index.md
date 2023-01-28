---
title: "iOS App – Film Blog (Part 4)"
date: "2013-07-09"
categories: 
  - "film-app"
tags: 
  - "ios"
---

So I need to test for an internet connection to make sure that I can download the JSON file with all the Film Reviews in it.

http://developer.apple.com/library/ios/#samplecode/Reachability/Introduction/Intro.html

https://github.com/tonymillion/Reachability

http://iosameer.blogspot.co.uk/2013/01/checking-internet-connection-in-ios-apps.html

Got it working using the last link, just as a quick test, will amend further.

Added Reachability.h/.m and added the SystemConfiguration.framework (this actually added to the correct folder!)

Reachability was made in 2010 so isn't ARC complient.

Go to **Targets** -> **Build Phases** -> **Compile Sources** and add

\-fno-objc-arc
