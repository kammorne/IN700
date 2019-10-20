---
layout: post
title: "Don't Use AJAX"
date: 2019-09-19
category: Classwork
tags: classwork project thingsnetwork orokonui webapp jekyll
---

# Don't Use AJAX
### It's not good for what we're after

After looking over the web app during the week, I found out why we may not have had any luck with the map getting information. After using a bunch of console.log() commands, we found that even though the AJAX
request was getting the data, as soon as we went to run the updateMap() function, the information was undefined. I began looking into solutions to fix this, and soon enough I found something that kind've worked.

The solution I had, (Although it didn't turn out to fully fix the issue), was to have the AJAX request in the updateMap() function. This actually let us access the data that was being requested by the AJAX ruquest, 
and it also meant that the information wasn't being lost.
