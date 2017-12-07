---
layout: post
title:      "Cookies and Sessions 101"
date:       2017-12-07 00:19:28 +0000
permalink:  cookies_and_sessions_101
---


I have had a difficult time grasping what sessions and cookies are, their purpose, and how they work together in the Rack web applications I create. If you are struggling to grasp these concepts as well, I hope this post will provide you with some clarity.

First off, you need to understand Hypertext Transfer Protocol (HTTP).  HTTP acts as a request-response protocol in our web applications, which means the user in a web browser requests information (ie: clicks on a link), the server processes the request, and then the server sends a response back to the user.  The other essential fact you need to know in order to undstand the role of sessions and cookies is that HTTP is a stateless protocol. This means that  HTTP does not store any information from the requests it receives, so it has no way of keeping track of the user that is making the requests.  A user would quickly leave your application because they would have to sign in each time they wanted to view a different page.  In order to remember a user through the duration of their time on your web application, you need to use cookies and sessions. 

Cookies save the data that the server sends back to the browser in each HTTP request.  Each "cookie is a hash that gets stored in the browser [or computer] and sent back to the server along with every subsequent request"(1). When you visit a website, register, and log in, that web application creates a cookie using your information and sends it back to your browser.  That personalized cookie is stored in your browser or computer and is sent back to the web server everytime you make a request to the web application.  There are two types of cookies, session and persistant.  Session cookies are stored in a user's web browser until the user logs out or visits another website. They allow the user to browse the web application without having to sign in everytime a new request is made to the server.  Persistant cookies are stored on a user's computer until they expire (if they expire) or "the user clears their browser's cache"(1). One thing they do is allow the user to be automatically logged in when they go back to the web application. 

A session is a hash that is accessible in your application's controllers, contains data about a user like their user_id, and "lives on the server"(1).  The user data that is stored in a session hash is sent to the user as a cookie.

Now, we need to discuss some ways the session and cookies work together in web applications.  As mentioned before, a web application stores data about a user in their session hash. This data is sent to the user as a cookie where it is stored in their browser or computer. Now, when a user is using your application they will not have to sign in everytime they make a new request to the server because the cookie is applied to the other web pages in your application. Also, if the user is shopping in your web application, the cookie stores what the user put in their shopping cart so the web application can remember what is in the users cart while they are still browsing.   Once the user logs out, the session cookies expire, but the persistant cookies remain stored on their computer.  When the user goes back to your web application, their computer sends the persistant cookie back to the web application server.  If the cookie matches the server's session hash data, then the user will be automatically logged in. 

Sessions and cookies are essential for every Rack web application.  Mentioned above are just a few examples of how they are used and why they are helpful.  Below are some resources I used to learn more about sessions and cookies that you may find helpful:





 *(1)Sinatra's session and cookies lesson in Flatiron's curriculum: https://learn.co/tracks/full-stack-web-dev-with-react/sinatra/sessions/sessions-and-cookies
 
 *(2) Sinatra's mechanics of sessions lesson in Flatiron's curriculum: https://learn.co/tracks/full-stack-web-dev-with-react/sinatra/sessions/mechanics-of-sessions
 
 *(3) Sinatra's sessions codealong lesson in Flatiron's curriculum: https://learn.co/tracks/full-stack-web-dev-with-react/sinatra/sessions/sinatra-sessions-codealong

*(4) http://webapps-for-beginners.rubymonstas.org/sessions/sinatra_sessions.html

*(5) https://developer.mozilla.org/en-US/docs/Web/HTTP/Cookies

*(6) http://rubylearning.com/blog/2009/09/30/cookie-based-sessions-in-sinatra/


