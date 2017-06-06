---
date: 2015-04-21 20:00:00+00:00
layout: post
title: Static Cells和Dynamic Prototypes (UITableView)
thread: 3
categories: UI
---

对于UITableView，最基本的设置是Content(内容)属性，它包含两个值：Static Cells和Dynamic Prototypes。Static Cells用来显示固定的单元格，内容呈现主要通过Xcode的可视化编程来实现，不需要额外的代码支持。Dynamic Prototypes为动态单元格，通过设定一个Cell模板，然后通过实现datasource接口和delegate接口的一些关键方法，从而动态生成表视图。

需要注意的是，Static Cells模式仅仅适用于表视图控制器(UITableViewController)，当你尝试设置标准视图控制器下的表视图(UITableView)content为Static Cells时，Xcode将提示一个错误：Static table views are only valid when embedded in UITableViewController instances。

另外：
viewForFooterInSection or viewForHeaderInSection 不调用会跟

是否为UITableViewStyleGrouped 、titleFor相关。。