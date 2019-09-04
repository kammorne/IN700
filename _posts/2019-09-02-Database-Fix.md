---
layout: post
title: "Database Fix"
date: 2019-09-02
category: Classwork
tags: classwork project thingsnetwork iotdata jekyll
---

# Database Fix

So Today, after researching over the weekend, I figured out how to fix the database information. The data entries going into the database had
to be the same as before, but the message information had to be changed to the new Things Network format. After changing this, the data was successfully
going into the database, and my Web App was collecting data again. All in all we only lost 2 weeks of data being stored, which in a real world scenario would
be catastrophic, and it's not much better for our project either. But I'm glad we're now saving data again.

Afterwards, Martin and I had a chat regarding the current Database Structure, and after some digging, we found out that all the data was being
saved in one Document, which was really bad for many reasons, one of which was that in order to get a single peice of data, we would need to read
every single entry in the database, which is slow and uses unnecessary bandwidth. So a solution to this would be to change over to a relational database,
such as MySQL, or completely rebuild the database structure for the nodes. I'd rather go to a SQL structured database, which gives us a lot more
usability, as well as using something a lot more people are comfortable with.
