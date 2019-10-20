---
layout: post
title: "Orokonui Web App Tinkering"
date: 2019-09-23
category: Classwork
tags: classwork project thingsnetwork orokonui web-app jekyll
---

# Web App Tinkering

So Today, we had Tony come in to look at what we had done for Orokonui, and although we had the data showing on the web app, it wasn't up to the standard that I wanted it to be. While he looked at the prototypes that 
the team had developed, I tinkered away at the web app, trying to get the map interface working correctly. I soon found out another issue with the implementation I had done last week. I found out that since it's an AJAX request,
which is Asyncronous, it was getting the data after the rest of the code was being run. I managed to fix this by changing the AJAX Request to run all the gate information updates inside the request function, which then meant that
the data that was being collected by the AJAX request was being instantly used instead of sitting like it was before. I had also optimized it so that it wasn't making the AJAX request for each gate, saving on bandwidth.

After the tinkering I had done, I finally got the map displaying a single gate's data over all of the labels on the map, which made it interesting when we were showing Tony, and once the gate was unlocked, all the labels went red,
rather than just the one the gate it was connected to.
