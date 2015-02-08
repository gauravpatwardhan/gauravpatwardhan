---
layout: post
title: OSX Hibernate / Deep Sleep Mode
---

So, I was looking this up sometime back and I thought that this might be a good place to start some OSX stuff.

Most of you will be using your OSX in the normal sleep mode. And that is good :) But sometimes I like my macbook to be in a so called "deep sleep" mode (similar to hibernate mode on Windows). To do that, open the Terminal and enter the following command:
```
sudo pmset hibernatemode 1
```
This will put your macbook in a sleep state similar to the one seen when you have very low and critical battery. To revert back to the original sleep mode enter the following command: 
```
sudo pmset hibernatemode 3
```
To see which mode you are currently in enter the following command:
```
sudo pmset -g | grep hibernatemode
```