---
title: "Google Maps iOS SDK - Error"
date: "2017-01-09"
categories: 
  - "ios"
tags: 
  - "googlemaps"
---

Google Maps iOS SDK

[https://developers.google.com/maps/documentation/ios-sdk/start](https://developers.google.com/maps/documentation/ios-sdk/start)

Followed the setup instructions using Cocoa Pods.

GoogleMaps (2.1.1)
GooglePlaces (2.1.1)

Built the Project and got the following error:

> Module 'GoogleMapsBase' not found

 

Added the following in:

> Target -> Build Setting -> Search Path-> Framework Search Paths

Add the following (+)

Framework Search Paths

 "${PODS\_ROOT}/GoogleMaps/Base/Frameworks"
 "${PODS\_ROOT}/GoogleMaps/Maps/Frameworks"

Build and Run.

* * *

Helpful Links

- [https://github.com/googlemaps/google-maps-ios-utils/issues/19](https://github.com/googlemaps/google-maps-ios-utils/issues/19)
- [https://github.com/googlemaps/google-maps-ios-utils/pull/20](https://github.com/googlemaps/google-maps-ios-utils/pull/20)
- [https://code.google.com/p/gmaps-api-issues/issues/detail?id=10190](https://code.google.com/p/gmaps-api-issues/issues/detail?id=10190)
- [http://stackoverflow.com/questions/19130629/framework-not-found-googlemaps-sdk-in-ios/19946503#19946503](http://stackoverflow.com/questions/19130629/framework-not-found-googlemaps-sdk-in-ios/19946503#19946503)
