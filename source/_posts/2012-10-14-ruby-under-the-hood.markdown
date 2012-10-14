---
layout: post
title: "Ruby under the hood"
date: 2012-10-14 17:29
comments: true
categories: 
---

After completing the computer architecture course at the University of Minnesota I find myself wondering about how things work at a low level. Now at the flatiron school we are covering ruby, and I find myself wondering how the memory allocation works for ruby objects. After a bit of searching I found this [slide deck](http://www.scribd.com/doc/27174770/Garbage-Collection-and-the-Ruby-Heap)that contained a very clear explanation of the behind the scenes workings of ruby; While paying special attention to memory allocation and garbage collection. 

These slides reminded me of my final project in the architecture class where I implemented a rudimentary malloc of my own which, it turns out, works much like the allocation of memory for classes works in ruby. I wonder how hard it would be to implement this method of garbage collection on top of it... hopefully nothing good on tv next weekend!
