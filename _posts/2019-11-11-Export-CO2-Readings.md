---
layout: post
title: "Exporting CO2 Readings"
date: 2019-11-11
category: Classwork
tags: classwork project thingsnetwork co2sensor jekyll
---

# Exporting CO2 Readings

Neville came and had a bit of a chat with us, and was quite intrigued with the CO2 sensors and the data they were sending, so he asked me if
it was possible to get a CSV file of the information covering the last week from the 4th. I agreed and went to get the data exported for him,
though that turned into a larger issue. So to catch up with the issue mentioned last post, I've continued getting in contact with the Dev Ops
team about the issue regarding our database virtual machine. Unfortunately, they mentioned that it may be a hardware issue, that they also
wouldn't be able to fix today since the server room that has the machine that the VMs are hosted is next to a room that was hosting an exam.

Luckily, it appears that getting access to the VM was a bit over the place, and it let us connect most of the time but then it would suddenly
freeze up and stop allowing connections. After dealing with this for almost an hour, I finally managed to get an SQL statement that would select
the data that Neville wanted. Finding this SQL statement wasn't exactly the easiest feat, and it also looks extremely janky, but it works.

The SQL Statement in question: `SELECT time, CONV(SUBSTRING(HEX(FROM_BASE64(payload)), 1, 4), 16, 10) FROM data WHERE app_id = "op_c02" AND time > "2019-11-04 23:59:59" ORDER BY data.time < SQL`

I had to go through this for the previous data because we weren't running a decoding function on the database, so any data being stored (excluding the
room sensors data) is still being stored in the Base64 format that it was sent in from the nodes.

