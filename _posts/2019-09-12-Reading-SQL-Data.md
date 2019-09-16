---
layout: post
title: "Reading SQL Data"
date: 2019-09-12
category: Classwork
tags: classwork project thingsnetwork iotdata jekyll
---

# Reading SQL Data

So today I went back to working on the iotdata webapp, which still wasn't reading any data from the database, even though it had a connection to the
database. I started to research how python works with SQL queries, and found out that it was very similar to how php works. After changing the current
queries in the webapp, I had the webapp reading data from the database, however I encountered a new issue. When loading a single node's data, I could
easily limit the search to 100 entries, which is what I want for the webapp. However, for the main page displaying all nodes, doing a simple sql limit 100
query on the data would only return 100 entries from one node. I tried a few different ways that I found online, however, the queries other people had tried
didn't work since they were using SQL server, where we are using MySQL, which has slightly different query statements.

I couldn't figure out how to sort this today, but decided to go home and research how to sort this out for the next class.
