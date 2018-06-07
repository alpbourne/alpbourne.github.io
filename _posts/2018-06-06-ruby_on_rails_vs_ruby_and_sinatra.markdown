---
layout: post
title:      "Ruby on Rails vs Ruby & Sinatra"
date:       2018-06-07 02:18:59 +0000
permalink:  ruby_on_rails_vs_ruby_and_sinatra
---


When making a web application using Ruby, one of the first decisions you will need to make is whether you will use Rails or Sinatra. There is no absolute right decision, it all depends on the nature of your app.  Hopefully the information below will make your decision a little easier. 

The first thing to consider is how large your app is going to be. Do you plan for your app to be used by 10 or 1,000s of users? Rails functions better with large scale apps than Sinatra does. However, Sinatra can be scaled up to handle larger apps, but it gets much more complicated to handle than if it were just created using rails. Often Sinatra apps that grow large end up being redone using Rails. 

Speed is another factor to consider. Sinatra is faster than Rails as long as it is being used in a small, simple application. However, the speed of Rails is still suited well for larger applications. 

Rails makes it easy to get an app running in a short period of time, so another factor to consider is your time frame. A new Rails app comes with a directory with files and folders that are automatically created. These make it extremely easy to get your app running on the web, but make can make it hard to debug if you are not familiar with what is in the automated directory. Sinatra is much simpler and will take longer to get your app running on the web, but will be easier to debug since you will code everything on your own.  

These are just a few quick points to help you make your decision. Take a look at the resources below for further information.

Resources
1) https://github.com/learn-co-students/what-is-sinatra-v-000
2) https://www.engineyard.com/blog/rails-vs-sinatra
3) https://devcamp.com/site_blogs/rails-vs-sinatra-frameworks
4) https://www.slant.co/versus/1233/10834/~ruby-on-rails_vs_sinatra
