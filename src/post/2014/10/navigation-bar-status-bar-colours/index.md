---
title: "Navigation Bar / Tab Bar / Status Bar Colours"
date: "2014-10-03"
---

http://www.appcoda.com/customize-navigation-status-bar-ios-7/

Add to .plist

`View controller-based status bar appearance: NO` `#define UIColorFromRGB(rgbValue) [UIColor colorWithRed:((float)((rgbValue & 0xFF0000) >> 16))/255.0 green:((float)((rgbValue & 0xFF00) >> 8))/255.0 blue:((float)(rgbValue & 0xFF))/255.0 alpha:1.0]`

`- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions { // Override point for customization after application launch. [[UINavigationBar appearance] setBarTintColor:[UIColor blackColor]]; //[[UINavigationBar appearance] setBarTintColor:UIColorFromRGB(0x067AB5)]; [[UINavigationBar appearance] setTitleTextAttributes:@{NSForegroundColorAttributeName: [UIColor whiteColor]}]; [[UINavigationBar appearance] setTintColor:[UIColor whiteColor]];`

\[\[UIApplication sharedApplication\] setStatusBarStyle:UIStatusBarStyleLightContent\]; return YES; }

Tab Bar `[[UITabBar appearance] setTintColor:[UIColor redColor]]; [[UITabBar appearance] setBarTintColor:[UIColor yellowColor]];`

Change the highlighted colour `[[UITabBarItem appearance] setTitleTextAttributes:@{ NSFontAttributeName : [UIFont fontWithName:@"HelveticaNeue-Bold" size:10.0f], NSForegroundColorAttributeName : [UIColor colorWithRed:0/255.0 green:138/255.0 blue:196/255.0 alpha:1.0],} forState:UIControlStateSelected];`

\-- `navigationBar.barStyle = UIBarStyleBlackOpaque;`
