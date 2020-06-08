---
layout: post
title:      "How to improve regular expressions"
date:       2020-06-08 02:04:11 +0000
permalink:  how_to_improve_regular_expressions
---

Regular expressions are what I consider to be a very annoying programming problem. Doing things without a regular expression library is slow and full of problems, but so is trying to use regular expression libraries simply because they are not user friendly. One of the simplest ways to make regular expressions better would be to make the shortcuts into words instead of characters. An example would be instead of the [a-zA-z] regular expression which would look for any character that has any lowercase letter or any uppercase letter. It would be nicer to read all_lowercase or all_uppercase although it is a lot more to type I don't know if it couldn't be an extra option. Most programmers are very good typers typing around 100 words per minute. I have heard that programmers don't write that many lines of code per day so I do not think that this bottle neck of writing a few more letters is such a big deal. Also there could be an automated way to make regular expressions using an automated user interface website so that a novice without regular expression coding knowledge could figure out how to easily make regular expressions. This would be hard to accomplish for very large regular expressions, but I think large regular expressions are already hard to accomplish anyways. Also the basic built-in python library re does not use a trie in order to make it go faster. A trie would make large regular expression usages quite a bit faster and it isn't hard to make. 

