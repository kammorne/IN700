---
layout: post
title: "Orokonui Web App Fixes 2"
date: 2019-11-18
category: Classwork
tags: classwork project thingsnetwork orokonui webapp jekyll
---

# Orokonui Web App Fixes 2

I also continued work on the Orokonui Web App, by changing the gates being shown on the app. The way we had it in the past was that the images
were just force-loaded when the page was loaded, and then afterwards just getting data from the database and showing it just wherever there was
room on the map.

The new way it works is by still forcing the images to be in the correct locations, (Which they actually weren't before, so that's fixed too), It
also has a hardcoded name, which is the same as the gate it's connected to. It then goes through the data it's collected from the database, before
checking the name of the gate from the database against the hard-coded name of the gate, and then setting it's closed state to what it collected from
the database.
