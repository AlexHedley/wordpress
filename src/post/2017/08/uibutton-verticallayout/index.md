---
title: "UIButton VerticalLayout"
date: "2017-08-04"
categories: 
  - "ios"
tags: 
  - "uibutton"
  - "uistackview"
  - "verticallayout"
---

https://stackoverflow.com/a/22621613/2895831

\[gist 87d1917da7745da9cd77033508e69243 /\]

I added some buttons into a UIStackView but the image overlaps the button.

\[gallery ids="1046,1047" type="rectangular"\]

I modified the _contentEdgeInsets_

CGFloat inset = (self.frame.size.height - totalHeight)/2;
self.contentEdgeInsets = UIEdgeInsetsMake(inset, 0.0f, inset, 0.0f);
