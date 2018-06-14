---
layout: post
title:      "Sass (Syntactically Awesome StyleSheets)"
date:       2018-06-13 21:27:41 -0400
permalink:  sass_syntactically_awesome_stylesheets
---

![](https://i.imgur.com/Bkwl5AK.png)

During my time at the Flatiron School, I learned how to customize the front-end of websites using CSS. Recently, a company I was interviewing with used Sass so I started learning it to prepare. I have become a fan of Sass since then! "Sass is an extension of CSS that adds power and elegance to the basic language."(5)

First off, it saves time! You can add variables, this alone can save a lot of time! Below you will see an example. The first box is the HTML, second is the SCSS(Sassy CSS), and third is the output. You will see the variables $text-color and $link-size. You can reuse these variables throughout your SCSS(Sass code) which makes it quick and easy to make edits. You don't need to go searching for every place you specified the link color when you want to change it. Now you just need to change it in one place. AWESOME! 

#### HTML
![](https://i.imgur.com/n52l7Lo.png)

#### SCSS
![](https://i.imgur.com/gfZsftH.png)

#### Output
![](https://i.imgur.com/F8gE3oj.png)

To build off of that, you can also build reuseable blocks of code which are called Mixins.  In order to create a Mixin, you need to define it like you see below. Then, you can use it by putting '@include the-name-of-your-mixin' inside the brackets of the selector you want the block of code in. That saves even more time!

#### Mixin
![](https://i.imgur.com/VozlpOo.png)

My other favorite part of Sass is the nesting feature.  You are able to nest your selectors so that it mirrors your html heirarchy. See the example below. To me, it makes it much easier to read.

#### Nesting
![](https://i.imgur.com/7BkStdf.png)

I've really enjoyed diving in and learning how to use Sass. The features mentioned above are pretty basic ones, but they can still make a big different in your code. I encourage you to look at some of the sources below that I used to write this blog for more information about Sass!


Sources
1. https://sass-lang.com/guide
2. https://scotch.io/tutorials/how-to-use-sass-mixins
3. https://alistapart.com/article/why-sass
4. https://www.sitepoint.com/sass-basics-nesting/
5. https://sass-lang.com/documentation/file.SASS_REFERENCE.html

