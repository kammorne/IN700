---
layout: post
title: "Exposure of Information"
date: 2019-04-08
category: Project
tags: project web-development iotdata webapp server python jekyll
---

# Exposure of Information

Today I found out that the repository that Martin created for the Iot Data webapp was public, and the app.py file contained sensitive information for logging in.
I've ended up fixing that problem, and began work on trying to format the data for all of the nodes saved in the database. However, I feel like I'm going to have
to find a different strategy for getting information from the database, as after a 'quick' test, it turned out the webapp would take 5 minutes to load the data and
display it to the screen. I feel like this wouldn't be acceptable as a final result, so I'm going to research better ways of accessing MongoDB, which will hopefully
take less time than what I've been using currently.
