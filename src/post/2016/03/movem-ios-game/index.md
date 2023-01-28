---
title: "Movem iOS game"
date: "2016-03-06"
categories: 
  - "ios"
  - "movem"
tags: 
  - "game"
---

So I found an implementation of an iOS Sokoban game

https://github.com/kennycason/swift\_boxxle

It's a year old so my first step was to update it.

I ran the Xcode updater then got to the left over errors.

@nonobjc var isPaused: Bool = false

Touches Began

override func touchesBegan(touches: Set<UITouch>?, withEvent event: UIEvent?)

let touch = touches!.first

CheckForWin

func checkForWin()

if ~isBoxOnGoal(box)

if !isBoxOnGoal(box)

I swapped out some images

Then i wanted to tile a background sprite

I found http://www.spritekitlessons.com/tile-a-background-image-with-sprite-kit/ then I converted it

\[gist id=b5e6ad227d988fe61327 file=TileSprite2.swift /\]

padNumber

let digits = countElements(String(number))

let digits = String(number).characters.count

Links

https://alexhedley.wordpress.com/2011/06/14/rw-beginning-iphone-programming-finished/ https://alexhedley.wordpress.com/2015/01/25/ios-maze-game-tutorial-initial-setup/
