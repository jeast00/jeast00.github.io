---
layout: post
title:      "My First CLI Project - Top Rated Beers"
date:       2020-06-24 17:09:01 +0000
permalink:  my_first_cli_project_-_top_rated_beers
---


So first things first, I felt like the world was on top of my shoulders and I honestly did not know what to do.  I knew that there were a lot of topics to use for a project like this, but I felt like I was way over my head.  I didn't know where to start... I didn't know what topic I wanted to do...  

The inspiration of moving forward and getting back on track was because of my daughter.  I knew that if I stuck with it, it will all come together at the end.  

I also felt like I have forgotten everything that I learned when I came to the portfolio project section.  lol.  I spent time reviewing sections I wanted to better understand.  I also reviewed the CLI walkthroughs from Avi to gain a better understanding of how to approach a CLI application.

I created a cli gem by typing gem and then the name of the gem I wanted created which was *top_rated_beers*.

So... I started where I would think that everyone has started... the setters and getters class.

I created a class called Beers which sets and gets all of the information needed to create an instance of that beer.

I then created a class called Scraper which would get a page and then get the details of that page.  I would then create class method called make_beers which would iterate from the get_beer_details class method and create instances of a beer.

Once I had the details created from the Scraper class, I created class methods to print the beer names and print the beer details.  

The beer names class method would iterate through the class variable @@all, and provide an index starting at 1 and output each beer in order numerically.  

The beer details class method would print the details of a beer that was selected by the user.

After the Beers class was completed, I started on the CLI class and created methods for calling the CLI class, looping through inputs until a certain command was used, and closing the app once that command was used.

I tested my code from beginning to end to ensure everything was working properly.  After I tested everything, I began refactoring my code, checking for any repetitions.  

I had a fun time working on this project and I look forward to making more projects in the future!


