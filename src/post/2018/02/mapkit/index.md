---
title: "MapKit"
date: "2018-02-03"
categories: 
  - "mapkit"
tags: 
  - "ios"
coverImage: "maps_ios-128x128_2x.png"
---

So I've been learning [MapKit](https://developer.apple.com/maps/) this week.

- [Developer](https://developer.apple.com/reference/mapkit)

It's been a fun new framework to look into.

Create an Annotation so you can have custom properties.

@interface Annotation : NSObject<MKAnnotation>

Add a category to it so you have a way of telling what it is.

This could be an enum.

In the Delegate method

\- (MKAnnotationView \*)mapView:(MKMapView \*)theMapView viewForAnnotation:(id <MKAnnotation>)annotation

You can use the category to set up some properties like a button and the pin colour.

I'm wondering if the "reuseIdentifier" should be unique here too?

You've added a button, now how to call it?

You could add a target and action

\[rightButton addTarget:## action:## forControlEvents:UIControlEventTouchUpInside\];

but instead you can use the "calloutAccessoryControlTapped" delegate method.

\- (void)mapView:(MKMapView \*)mapView annotationView:(MKAnnotationView \*)view calloutAccessoryControlTapped:(UIControl \*)control

As this isn't a  "MKAnnotation" like "viewForAnnotation" but an "MKAnnotationView" we need to get the annotation from the passed view.

if (\[view.annotation isKindOfClass:\[OotAnnotation class\]\]) { ... }

Then call pfs,

Then in the "prepareForSegue" you need to get the Annotation when you click on a Pin button, this can be cast from the Sender

if (\[view.annotation isKindOfClass:\[OotAnnotation class\]\]) { ... }

Annotation \*annotation = (Annotation \*)\[(MKAnnotationView \*)sender annotation\];

You could then pass your custom Location details via the ViewController. (See code)

\---

Searching for locations to add to the map:

MKLocalSearchRequest

\---

Adding a route, need to investigate this more.

MKPolyline

\---

All Code

\[gist 6ac1c60428f6e13692f7f3f11d931f0e\]
