--- 
layout: post
title: "About Rails Depoly"
date: 2012-08-07 23:57:31 +1000
guid: urn:uuid:05e387ce-f6ea-4079-a498-f7bb9e06f731
tags:
  - rails
  - mongodb
---

This topic is about some general problems when I depoly rails app.

After I set up server environment, I cloned source code by git. Usually, we need do some steps to make sure it works on production environment.

gem we need install
> bundle install

initial mongodb
>rake db:seed

compile files we need for production
>rake assets:precompile --trace RAILS_ENV=production

install javascript runtime
>sudo apt-get install nodejs

or from package [src](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager)
> apt-get install make python g++

> mkdir ~/nodejs && cd $_

> wget -N http://nodejs.org/dist/node-latest.tar.gz

> tar xzvf node-latest.tar.gz && cd \`ls -rd node-v*\`

> make install
