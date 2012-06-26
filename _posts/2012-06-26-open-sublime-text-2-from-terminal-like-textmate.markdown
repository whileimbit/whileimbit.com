--- 
layout: post
title: "Open Sublime Text 2 from Terminal Like TextMate"
date: 2012-06-26 21:55:47 +1000
guid: urn:uuid:1b212649-9a63-4824-8c95-fd974e230fd9
tags:
  - sublime text
  - editor
  - tips
---

I used to run below command from terminal to open current projects in TextMate.

	mate .

Now I am swiching to [Sublime Text 2](http://www.sublimetext.com/). Which is missing this. What I need to do just add below code into `~/.bash_profile`

	alias sub='open -a "/Applications/Sublime Text 2.app"'
	
Then I can open projects the same you would have in TextMate in Sublime Text but with the following command

	sub .

That means you also can open any app from terminal, like when I want to edit markdown post in jekyll, or edit README file in my project from terminal by Byword:

	alias bw='open -a "/Applications/Byword.app"'
