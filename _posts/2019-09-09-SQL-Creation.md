---
layout: post
title: "SQL Creation"
date: 2019-09-09
category: Classwork
tags: classwork project thingsnetwork iotdata sql jekyll
---

# SQL Creation

So today I started looking into creating an SQL database for all our data. The main reason for changing to SQL is that most people know how to
use SQL since most people would have done Databases 2 last year, compared to the Mongo Database where people would have to research it before 
being able to do anything with it. So we started discussing how to set up the database. We figured we would be able to use a MariaDB login on the
polytechnic network, but after talking to both the Dev Ops team (who didn't have access to Maria) and Rob (who convinced us that using the polytechnic
network may cause problems in the future with how much data we're saving.) We decided that we would run our own MariaDB instance in the VM that held
the Mongo Database. Rob recommended a few tutorials online for setting it up, and after a short amount of time, we managed to get a basic SQL server
running on the VM.

The next task I had to do was to convert the iotdata webapp to use SQL instead of the MongoDB connections. This didn't cause too many issues when changing
over, however I did experience some issues with the connection, due to the current firewall settings on the VM. After doing a bit of research, plus changing
some settings for the MariaDB database, we managed to get a connection to the database from the webapp, and Henry got the data from the Things Network going
into the database.
