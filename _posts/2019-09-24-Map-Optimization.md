---
layout: post
title: "Map Optimization"
date: 2019-09-24
category: Classwork
tags: classwork project thingsnetwork orokonui web-app jekyll
---

# Map Optimization

So today I wanted to optimize the map and fix the prototype issues we were having yesterday. I changed the SQL query to select all of the gates, instead of only one of them, but that instantly threw an error regarding decoding the
information. I looked at the query on phpMyAdmin and found out that the query I had written was selecting the earliest entry from each gate, which meant that some of them had un-decodable payloads, which was making my code for getting
the gate's state break the site. I asked some of my classmates who were taking Databases 3 if they had any idea where I was going wrong with the query, and they even went and tried creating some queries themselves, as well as asking Krissi
if she knew how to achieve what we wanted, but unfortunately, they could not find a solution with how we had the database set up.
