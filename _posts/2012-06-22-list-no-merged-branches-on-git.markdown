--- 
layout: post
title: "List no merged branches on git"
date: 2012-06-22 09:20:51 +1000
guid: urn:uuid:db375aa9-b9f1-4815-94fd-e725f94ef2c4
tags:
  - git
---

We are using [git-flow](http://nvie.com/posts/a-successful-git-branching-model/) as git branching model to do development.

However, there are more and more feautre branches were generated, and we need to make a list quickly for all branches to see which branch is still under development and not merged into master branch sometimes.

Then this command will give a huge help.

> git branch --no-merged master

And if add `-a` you can get all include remote branches.