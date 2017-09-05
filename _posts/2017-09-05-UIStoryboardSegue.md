---
date: 2017-09-05 20:00:00+00:00
layout: post
title: UIStoryboardSegue
thread: 3
categories: UI
---
①自动segue： 
直接从相应的控件连线到相应的ViewController，然后选择push 
![说明文本][1](UIStoryboardSegue手动segue.jpeg)

②手动segue： 
从登陆界面连线到相应的ViewController，然后选择push。 
￼
然后在响应的事件中添加如下代码：
- (IBAction)clicktoTwo:(id)sender {  
	 [self performSegueWithIdentifier:@"oneToTwo" sender:nil]();    
}  

[1]:	UIStoryboardSegue%E6%89%8B%E5%8A%A8segue.jpeg
