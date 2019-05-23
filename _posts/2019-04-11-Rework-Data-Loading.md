---
layout: post
title: "Rework Data Loading"
date: 2019-04-04
category: Project
tags: project web-development iotdata webapp server python jekyll
---

# Rework Data Loading

Currently Reworking the parsing information from the db to the website, as due to what happened on Monday, I figured it wouldn't be acceptable for a webapp to take 5
minutes to load the information from the server, every time you load the webpage. I've changed it so the webapp loads the data when it's first turned on, and then simply
grabs the required data when the page is loaded. Currently I'm testing to see if that works.

![Reading Data](https://kammorne.github.io/lagoma1_IN700/img/evidenceReadingData.jpg)
