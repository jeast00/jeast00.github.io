---
layout: post
title:      "Sinatra Project - My Game Collection"
date:       2020-08-23 14:22:26 +0000
permalink:  sinatra_project_-_my_game_collection
---


There's always a point in time when you are trying to figure out what you want to do, especially in life.  When I was approaching the Sinatra project, I had absolutely no idea what I wanted to do.  I had many ideas come to mind, but at the end of it, my true passion overcame all others... 

Games!

I've been a gamer my entire life.  From video games to board games to basically anything gaming, I have always enjoyed playing them.  

Thus brings us to my sinatra project - My Game Collection

I reviewed a bunch of videos and lectures and even googled (is that even a word? lol) everything I needed to know for this project.  The project required a registration (sign up) for a new user, and the ability to login and log out that user.  I reviewed all lectures consisting users, how to set up controllers, how to handle each users session when logged in.

I used a gem called 'corneal' which sets up the file structure for a sinatra application. The rest is up to the developer to add in the code for their project.  The MVC (Models Views Controllers) for my project was set up handling each file separately in a folder.

For example,

My Controllers folder had an Applications Controller which was being inherited by the Sinatra::Base.  Then I had three other controllers: Users Controller - handled the users ability to edit, delete, and logout of their account; Sessions Controller - handled the ability to create a new user (sign up) and login once user has signed up; Games Controller - handled the ability to create, read(show), edit(update), and delete a game by that user.  

I had two Models for my project, User and Game.  User was being inherited by the ActiveRecord::Base handling methods - has_secure_password (which has the ability to check the authenticity of a password being used when a user is logging into their account) and has_many :games - ability to have more than one object(game) added to the database to that user.  Game was being inherited by the ActiveRecord::Base handling the method belongs_to :user - ability that adds data to that specified user.  

My Views were separated for each controller showing the pages for signups, logins, welcoming the user, if first time, welcoming back the user if they had an account and were able to log in, checking validations for deleting accounts, deleting games from their collection, and logging out.  

This project was definitely alot of fun creating it and alot of fun researching ways on how to code it.  I definitely learn alot on ActiveRecord and Sinatra, and I could not get over the fact of how simple utilizing ActiveRecord and Sinatra was for this project.  

I'm excited to see what Rails has for us in the next module!


