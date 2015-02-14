---
date: 2015-02-14 04:56:47+00:00
layout: post
title: UITabbarController 要点
thread: 3
categories: UI
---

**如果想完全自定义TabBar**  

    UIImage *voidImage = [[UIImage alloc] init];
    [[UITabBar appearance] setBackgroundImage:voidImage];
    [[UITabBar appearance] setShadowImage:voidImage];
    self.tabBar.selectionIndicatorImage = voidImage;
    
    self.customTabBar 初始化;
    [self.tabBar addSubview:self.customTabBar];  
  
**巧妙使用系统封装的UI**

	   // Set Tab Bar Item
      self.tabBarItem = [[UITabBarItem alloc] 	 initWithTabBarSystemItem:UITabBarSystemItemContacts tag:1];
        
       // Set Badge Value
      [self.tabBarItem setBadgeValue:@"12"];
...未完待续