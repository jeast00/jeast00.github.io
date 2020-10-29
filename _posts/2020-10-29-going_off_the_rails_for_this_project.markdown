---
layout: post
title:      "Going off the 'Rails' with this project"
date:       2020-10-29 11:15:26 -0400
permalink:  going_off_the_rails_for_this_project
---


When I started working on my Rails project, I knew I wanted to extend my sinatra project of "MyGameCollection" with an additional model for associations.  I had three models set up, User, Game, Genre with my join table being the Genre.  Database tables were set with the join table's foreign keys.  I had Faker gem data seeded to check the associations and everything was working properly and accordingly.  

I decided to move on to Omniauth, because I thought that having a third party log in was going to be tough and I wanted to make sure I had everything working with the log in.  It was tough.  I was constantly running into issues with Omniauth.  I watched videos, read up on anything new that could have been missed and was still getting errors.  

Since I wasn't able to figure out why Omniauth wasn't working, I started working on the views (forms) for my project.  I kept checking associations in rails console to make sure they were working properly, but for some logical reason, they were not matching up correctly and being displayed properly in the views.  Typically at this point, I was getting frustrated and needed to take a break from coding.  

It wasn't until yesterday, after submitting this post, that I realized my model associations were backwards.  I realized that my associations did not make any sense.  I updated my associations and check them with the Faker seed data.  

Omniauth was still giving me issues, until I found out that debugging will become your best friend.  I used the gem 'byebug' to check on the third party login and realized that the 'info'rmation being passed through was not set up correctly when validating or creating a new user.  With a sigh of relief, I was able to debug the issues I had with Omniauth and now have it working in my project.

With the countless hours of coding, sleepless nights, and a better, confident way to debug my code, I feel like I have gotten back on the 'Rails' with this project.
