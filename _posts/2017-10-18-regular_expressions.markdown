---
layout: post
title:      "Regular Expressions"
date:       2017-10-18 19:02:33 -0400
permalink:  regular_expressions
---


When Regular Expressions were first introduced in the curriculum, I had a very hard time grasping their role and how to create one.  In order to understand this concept, I had to sit down and read chapter the about Regular Expressions in "The Well-Grounded Rubyist" written by David A. Black.  In basic terms, I learned that Regular Expressions are powerful, pattern-matching tools used in every programming language.  The Regular Expressions are instances of the Regexp class in Ruby and made up of character patterns inside of a pair of forward slashes.  The character patterns look for matches in the strings they are applied to (Black 331).  Even if you do not enjoy using Regular Expressions in your own code, you should be able to understand them if you come across one in another programmer's code.  Below are a few examples of how you can use Regular Expressions in your own code:
### The Dot (.)
![](https://imgur.com/n5VgBse.jpg)

The dot (.) is a wildcard character. The (.) is used to match any character, except a new line. In the example above, you can see that "night" and "fight" were correctly matched.  However, if "%ight" or "5ight" was in the string, it would be found as a match as well since (.) matches any character (Black 334).
### Character Classes
![](https://imgur.com/tSTrJOV.jpg)

To eliminate the possibilty of matching "%ight" or "5ight" in the example above, we are going to use a Character Class. A Character Class is a list of characters grouped together by square brackets  inside a Regular Expression (Black 334). In our example, the list of characters only allow the regular expression to match a "n" or "f" that is followed by "ight."
### Named Captures
![](https://imgur.com/OpTFuEs.jpg)

Named Captures are a way to label subexpressions. In the above example, we are taking the string and splitting it into two parts, :first and :last, using parenthesis. This makes the string more useful to us. If we only needed someone's first name, we now have a way to access it without having to include the last name as well.

**Source:**
Black, David A. “Regular expressions and regexp-Based string operations.” *The Well-Grounded Rubyist*, 2nd ed., Manning Publications Co., 2014, pp. 330–359.
