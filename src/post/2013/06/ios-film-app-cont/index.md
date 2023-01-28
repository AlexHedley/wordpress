---
title: "iOS App - Film Blog (Part 2)"
date: "2013-06-29"
categories: 
  - "film-app"
tags: 
  - "ios"
---

So I've been working on it a little more tonight,

I've added the Star Ratings now.

[![Film List with Star Rating](http://alexhedley.files.wordpress.com/2013/06/screen-shot-2013-06-29-at-23-33-59.png?w=159)](http://alexhedley.files.wordpress.com/2013/06/screen-shot-2013-06-29-at-23-33-59.png)

Copied

return \[UIImage imageNamed:@"1StarSmall.png"\];

for each one, changed all the numbers from 1 to 2 to 3 etc but forget to change Star to Star**s**, couldn't work out why it wasn't working, the String comparison was working, checked other things, nothing seemed to be fixing it, of course don't have any 1 Star Ratings or it would have shown up, or if I'd copied a line other than the first to return another image.

Oh well, lets learn and move on.
