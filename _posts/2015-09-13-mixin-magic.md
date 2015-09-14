---
layout: post
title:  "Mixin Magic"
date:   2015-09-13 
excerpt: Enjoy a fewer keystroke kind of life. 
---

I'm sharing this mixin for 2 reasons.  
<br>
1. I never want to lose it, and I've learned that the best way for me to never lose things is to write them down.  
<br>
2. I want to share this tool with all of you.  
<br>
This mixin is one that allows you to state your font-size in your style sheet without having to write a fallback in pixels. Just put this at the top of your scss and the amazing Internet will automatically record the pixel fallback for you. No more writing multiple lines of code to declare a single font-size.   
<br>

<br>
	```	@mixin font($em) {
    	font-size: ($em*16) + px;
    	font-size: ($em) + em;
	}
	```  
<br>
Write it as:  
	```h1 {
			@include font(2);
	 	}
	 	```  
<br>
That's it! Enjoy a fewer keystroke kind of life. 

