---
layout: post
title:      "Movie Bucket List with  jQuery Front End"
date:       2018-03-12 21:34:40 -0400
permalink:  movie_bucket_list_with_jquery_front_end
---


![](https://imgur.com/FWbbkY2.jpg)

In my last post I introduced my app **Movie Bucket List**.  As a review, It is an app designed to help you keep track of all the movies you want to see. Users create Bucket Lists where they can store their must-see movies. Since that last post, I have added a few things like a jQuery Front End and the ability to create comments for Bucket Lists. 

When I first started thinking about how to implement my jQuery front end, I had a slightly difficult time deciding how to meet the requirements in a way that would enhance my app. I wrote out a few different diagrams in my notebook to help me visualize it and come up with a plan. The first decision I made was to create a Comments model that belonged to Bucket Lists. Using the Comments model, I was able to include an index resource that is rendered using jQuery and an Active Model Serialization JSON backend. When a User is in the show page of a Bucket List they can click 'Load Comments' and all the comments for that Bucket List will appear below. On the Bucket List show page a User is also able to create a new comment. When creating a new Comment, it creates a JS Comment model object that has a renderComments method on the prototype. If the User clicks load comments and then creates a new comment, they will see the new comment added to the list above without a page refresh. The second decision I made was to render the Movie show resource under each Movie on the index page using jQuery and an Active Model Serialization JSON backend. A user is able to click 'Details' and the individual movie's show page that was clicked will appear underneath.

This was another great learning experience for me. Last time I said I was hesitant to say this app is finished, because I still saw more potential for it. I still agree with that, but am happy with the progress. 
