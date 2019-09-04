---
layout: post
title: "Database Discovery"
date: 2019-08-29
category: Classwork
tags: classwork project thingsnetwork iotdata jekyll
---

# Database Discovery

So today I made the discovery that the database webapp I had developed last semester had become completely obsolete due to the Things Network
switchover. Because of how the Things Network sends data, the database wasn't getting any data from the nodes. I had to delve into the MongoDB
Virtual Machine and have a look at how the database was receiving items, and then saving to the database. After talking with Henry for a bit, we
found out that it would be easily fixed with a few name changes in the file, as well as a topic change. However, after doing so, the virtual machine
would pick up the node data, but not save it. I was stumped and decided to go home and research why it wouldn't be working.
