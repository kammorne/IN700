---
layout: post
title: "Removing Hardcoded Data"
date: 2019-09-16
category: Classwork
tags: classwork project thingsnetwork orokonui web-app jekyll
---

# Removing Hardcoded Data

So today we had another meeting to decide what we were gonna do for the next 2 weeks before the holidays. We decided we needed to focus on getting data from the database onto the orokonui web app, so
I was tasked with doing that. Bee and I began looking into how the app actually got data already, and found out that most if not all of the data on the web app itself was all hardcoded, which actually
made it easier, since we didn't have to alter the already existing code for it to work. We began tinkering with the data page on the web app, and soon enough, we got a basic query to get an entry from
the database for the prototype gate that Bee had created. With that being done, we began looking at how to get the data to the map. Unfortunately, this is where we got stuck, we tried many different options,
but for some reason I could not get the map to update with the required information, even though we were using an AJAX request to get the information from the database.
