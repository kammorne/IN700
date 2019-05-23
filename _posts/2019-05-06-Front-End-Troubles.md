---
layout: post
title: "Front End Troubles"
date: 2019-05-06
category: Project
tags: project web-development iotdata webapp server python html jekyll
---

# Front End Troubles

Got the data moving to the front end, however decoding it from the JSON file returns undefined in all fields. Another problem I encountered was limiting the amount of data going through from the backend.
Unfortunately, the data is stored in segments, depending on the device, so using the .limit() function that is included with MongoDB only limits the amount of devices being selected from the database.
I think I've come up with a solution however, but I'll have to implement it later. I've got to tend to other classwork.
