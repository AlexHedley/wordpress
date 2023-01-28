---
title: "Marvel API"
date: "2015-08-16"
---

So I found that Marvel have an API.

**Marvel API** [http://developer.marvel.com/](http://developer.marvel.com/) _Community_ [http://developer.marvel.com/community](http://developer.marvel.com/community) _Authorization_ [http://developer.marvel.com/documentation/authorization](http://developer.marvel.com/documentation/authorization)

Original [https://gist.github.com/oshliaer/eb8d7197e6749475652a](https://gist.github.com/oshliaer/eb8d7197e6749475652a)

\[gist 2726b33578720c42b24c /\]

I converted them to version 2 as I only have 2.7 on my machine atm

Convert from 3 to 2 [https://pypi.python.org/pypi/3to2/1.1.1](https://pypi.python.org/pypi/3to2/1.1.1)

3to2 -w FILENAME.py

**MD5** [http://www.miraclesalad.com/webtools/md5.php](http://www.miraclesalad.com/webtools/md5.php)

The [Authorisation](http://developer.marvel.com/documentation/authorization) page shows:

ts: 1

Public Key: 1234

Private Key: abcd

making: 1abcd1234

hash: ffd275c5130566a2916217b101f26150

(http://gateway.marvel.com/v1/comics?ts=1&apikey=1234&hash=ffd275c5130566a2916217b101f26150)

I created a Mac App to create the Hash and create this URL.

[http://stackoverflow.com/questions/2018550/how-do-i-create-an-md5-hash-of-a-string-in-cocoa](http://stackoverflow.com/questions/2018550/how-do-i-create-an-md5-hash-of-a-string-in-cocoa)

NSTimeInterval timeStamp = \[\[NSDate date\] timeIntervalSince1970\];
// NSTimeInterval is defined as double
NSNumber \*timeStampObj = \[NSNumber numberWithDouble: timeStamp\];
txtTimestamp.stringValue = \[timeStampObj stringValue\];

I call this in the app and it doesn't work.

[https://developer.apple.com/library/mac/documentation/Cocoa/Reference/Foundation/Miscellaneous/Foundation\_Constants/index.html#//apple\_ref/doc/constant\_group/URL\_Loading\_System\_Error\_Codes](https://developer.apple.com/library/mac/documentation/Cocoa/Reference/Foundation/Miscellaneous/Foundation_Constants/index.html#//apple_ref/doc/constant_group/URL_Loading_System_Error_Codes)

NSURLErrorUserAuthenticationRequired = -1013
NSURLErrorDomain Code=-1013

I can't get the MD5 from Python to match the ObjC one.

I can't get it to work with [CocoaRestClient](http://mmattozzi.github.io/cocoa-rest-client/) or ObjC.

Then I realise I've got my keys swapped, d'oh!
