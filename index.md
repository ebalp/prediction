---
title       : A word prediction app
subtitle    : 
author      : Enrique Balp
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Word Prediction 

In today's world people type many different phrases in many devices. 
It is important to predict the next word so in order to have functions such as autocomplete. Features based on word prediction have the potential of adding value.

In this presentation we show a word predicting app we just developed.

---

## The Data

For the model, we used data from Twitts, News and Blogs, taken from the HC Corpora English corpus. Consisting on more that 500 MB of text, we believe this is representative of the use of modern English language.

---

## The algorithm

After removing all characters except alphanumeric and apostrophes, we created 2-grams, 3-grams and 4-grams. 
Then we counted the occurrences of each n-gram and sorted them in descending order.
After getting an input string, we see if it is better to use the 4-grams, 3-grams or 2-grams.
Given this, we are now in a position to give the probabilities for each prediction (based on n-gram count).

---

## The app

The app accepts an input string and a number of desired predictions (will give less if there are not enough).

It outputs the most likely word based on the model and a table with the probabilities for different predictions.

--- 

## The future

There are many possible improvements of the algorithm and the app.
For example, we could include 5-grams to give better predictions. 
Also the input string now doesn't handle well special characters.

Nevertheless, we are on the path to a great word prediction tool, which could possible add great value in autocomplete functions everywhere.


---


