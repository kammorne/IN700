---
layout: post
title: "Orokonui Web App Fixes"
date: 2019-11-14
category: Classwork
tags: classwork project thingsnetwork orokonui webapp jekyll
---

# Orokonui Web App Fixes

So after our trip to Orokonui, I decided that I wanted to do some fixes that I had in mind for the Orokonui web app, which were bugging me for
a while. The first one which I decided to tackle today was the routes on the app, since I believed one of the routes was causing the map not
to load unless you were in the /home URL on the app. (Spoiler alert: It wasn't a route).

After tinkering with the app and discussing with the team about which routes we needed, I removed the map tab, alongside the contact us tab, since
both were rather redundant (and the contact us tab didn't even work). After that I looked at the scripts for the map, and realised that the issue
with the map not loading unless you were on the /home URL was because of a implementation I had done earlier in the semester to prevent the console
from spewing errors about the map being unable to load when not on the correct page. I implemented it like that due to the app being designed by every
page loads the same Javascript files, rather than just having the needed Javascript files on the required views.
