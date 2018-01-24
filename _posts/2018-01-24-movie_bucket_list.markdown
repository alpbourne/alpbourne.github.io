---
layout: post
title:      "Movie Bucket List"
date:       2018-01-24 17:41:25 +0000
permalink:  movie_bucket_list
---


For my Rails Final Project, I created the app Movie Bucket List.  There have been many times I say to myself "Man, I need to see that movie," and then I never end up watching it because I forget or can't remember the title. That is where my app Movie Bucket List comes quite handy. It is a Rails app designed to help you keep track of all the movies you want to see. Users create Bucket Lists where they can store their must-see movies. If a User is unable to find the movie they want to see in the app, then they can easily create a new movie to add. Once a User has watched one of their movies, they can edit the bucket list and check off that movie as seen. Another thing to note is that if a user adds a movie, it will then be available for all other users to edit or add to their own Bucket Lists. This allows all users to correct any errors they find and creates an expansive library of movies to choose from.

This project was definitely a growing experience for me. I was stretched a lot. I was quite overwhelmed trying to figure out how to meet the requirements with an interesting app idea. First, I wrote out on paper what my models were going to be and their attributes. Then, I figured out their relationships with each other. Once those were written down in my notebook, I added those to my app. After the models were added to my schema, I used Devise and OmniAuth to set up the user log ins of sign up, sign in, and sign in with facebook.  I knew I needed data to play around with so I seeded some movies into the app. From there I created a show page index of all the movies. From that point on, I gradually added features in the model controllers and view pages that I saw fit for the app.  After I felt all my functionality was working properly, I added partial forms in the Movies and Bucket Lists views to make it more DRY.  

I really am greatful for this experience, out of all the previous projects, this one stretched me the most. I learned to reach out and not be ashamed to ask for help and another set of eyes. From those moments of reaching out, I learned new tools to debug and grasped a greater understanding of what is going on under the hood of my code. I think the hardest part of the process was getting all of my nested attributes and forms to work and understanding all the variables getting passed around in the forms and controllers. I am hesitant to say this app is finished, because I still see more potential for it and I love that! 
