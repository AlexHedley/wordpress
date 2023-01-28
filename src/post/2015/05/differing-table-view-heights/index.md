---
title: "Differing Table View Heights"
date: "2015-05-03"
categories: 
  - "ios"
tags: 
  - "height"
  - "tableview"
---

So I'm creating an app which I wanted different themes for the Table View. I've created two Prototype Cells and given them different CellIdentifiers. This is then stored in a plist of DefaultPreferences.

Even though I'd given them different heights in IB but this wasn't reflected in the app.

\[gist 6218ba01a2e8fc3ef0b5 /\]

Then once you've made your choice and you return to the List you'll want to reload the data.

\-(void)viewWillAppear:(BOOL)animated {
    \[self.tableView reloadData\];
}
