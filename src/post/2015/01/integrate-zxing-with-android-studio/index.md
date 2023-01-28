---
title: "Integrate Zxing with Android Studio"
date: "2015-01-28"
categories: 
  - "android"
tags: 
  - "android-studio"
  - "zxing"
---

Spent some time trying to integrate [Zxing](https://github.com/zxing/zxing/) into my app and couldn't get the Activity to work.

Lots of posts saying add this activity but the name was linked to their project so didn't work.

Do i add it in via the Project Structure, do I compile the jar using maven.

Nothing seemed to work.

I asked on the TeamTreehouse Forum and got a reply,

https://teamtreehouse.com/forum/adding-an-external-library-to-an-android-studio-project

http://stackoverflow.com/questions/18543668/integrate-zxing-in-android-studio

I think I'd come across that SO answer but as I'd been going back and forth trying everything had overlooked it.

https://github.com/journeyapps/zxing-android-embedded

Tried again and got it working.

\[gist e7374ab15ebd3722e904 /\]
