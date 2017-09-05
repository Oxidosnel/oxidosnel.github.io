---
date: 2017-09-05 20:00:00+00:00
layout: post
title: UIStoryboardSegue
thread: 3
categories: UI
---
①自动segue： 
直接从相应的控件连线到相应的ViewController，然后选择push 
![][image-1]
②手动segue： 
从登陆界面连线到相应的ViewController，然后选择push。 
￼
然后在响应的事件中添加如下代码：
- (IBAction)clicktoTwo:(id)sender {  
	 [self performSegueWithIdentifier:@"oneToTwo" sender:nil]();    
}  



[image-1]:	images/UIStoryboardSegue%E8%87%AA%E5%8A%A8segue.jpeg