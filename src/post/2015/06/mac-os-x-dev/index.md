---
title: "Mac OS X - Dev"
date: "2015-06-09"
categories: 
  - "macosx"
---

I bought:

[https://www.bignerdranch.com/we-write/cocoa-programming/](https://www.bignerdranch.com/we-write/cocoa-programming/)

I've got version 3, 4 & 5.

Working through 4 now as it's ObjC.

I'm going to document things I've had to look up.

Chapter 2

Probably look back and say why didn't I spot this but it should help it not happing again:

Unknown type name 'NSTextField'

```
#import <Cocoa/Cocoa.h> 
```

Could have just added a .pch file

Project Settings Under the 'Apple LLVM 6.0 - Language' section in the 'Prefix Header' I added "<PROJECTNAME>/<PROJECTNAME>-Prefix.pch"

![h](images/h.png)Random-Prefix.pch

```
#ifdef __OBJC__
#import <Cocoa/Cocoa.h>
#endif
```

.
