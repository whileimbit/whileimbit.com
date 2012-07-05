--- 
layout: post
title: "Command to start Sublime Text on Ubuntu"
date: 2012-07-05 15:17:37 +1000
guid: urn:uuid:bdb189bd-269c-4b99-88d7-254566ca550f
tags:
  - sublime text
  - tips
  - ubuntu
---

There is a quick [method](http://whileimbit.com/2012/06/26/open-sublime-text-2-from-terminal-like-textmate.html) to open Sublime Text from Terminal on Mac OS X.

This is how to run Sublime Text on ubuntu terminal.

Create command file:

	sudo vim /usr/local/bin/subl

Copy & Paste below code, and change to your Sublime Text path

	#!/bin/sh
	$HOME/Apps/Sublime\ Text\ 2/sublime_text $1 &
	
Give execute permission

	sudo chmod +x /usr/local/bin/subl

Then you can do like this

	subl .
	
or 

	subl filename
	

