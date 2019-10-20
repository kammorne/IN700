---
layout: post
title: "Map SQL Queries"
date: 2019-09-26
category: Classwork
tags: classwork project thingsnetwork orokonui webapp jekyll
---

# Map SQL Queries

So today, I continued to tinker with the SQL Query that I had been working on on Tuesday, and after 20-30 minutes of trying different options, I finally managed to get an SQL query that worked how I wanted it to. I then proceeded to update the
Javascript so that all the gates would display the new information, but for that to work without errors, I had to limit the gates to 5 instead of 6, since we don't currently have enough boards to create another gate prototype for them all to show up.

![UpdateMap](https://kammorne.github.io/lagoma1_IN700/img/MapUpdate.png)

After I got the map working, I began working with some of the javascript files trying to prevent some console errors. Unfortunately, the way that James set up the web app, he had it so that every html page uses the same JS files, meaning that on
one page, it would try to load the map when the map isn't there, and on another it would try to load the graphs for the data, but there's no container for the graphs.

I fixed the map error by having a location check on the JS file, so that the code only runs if the user is on the correct page. This isn't the best solution, but it works for now until I can find a new solution.
