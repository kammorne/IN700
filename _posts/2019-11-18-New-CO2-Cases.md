---
layout: post
title: "New CO2 Cases and Orokonui Web App Work"
date: 2019-11-18
category: Classwork
tags: classwork project thingsnetwork co2sensor orokonui webapp jekyll
---

# New C02 Sensor Cases

So Today I wanted to tackle the issue with the CO2 Sensor cases, which wasn't really an issue, but something I wanted to do for showcase
more than anything. The main thing was that the cases were just repurposed room sensor cases, and because of this, the holes on the box
didn't quite line up, which on one of the boxes was blocking one of the sensor pads on the CO2 sensor. So I redesigned the cases to have
slightly different holes on the front, as well as the box stating "CO2" on the top of the box. I also widened the hole for the charging port
so that it would work with the resoldered boards, since they were slightly different than the room sensor boards.

# Orokonui Web App Fixes 2

I also continued work on the Orokonui Web App, by changing the gates being shown on the app. The way we had it in the past was that the images
were just force-loaded when the page was loaded, and then afterwards just getting data from the database and showing it just wherever there was
room on the map.

The new way it works is by still forcing the images to be in the correct locations, (Which they actually weren't before, so that's fixed too), It
also has a hardcoded name, which is the same as the gate it's connected to. It then goes through the data it's collected from the database, before
checking the name of the gate from the database against the hard-coded name of the gate, and then setting it's closed state to what it collected from
the database.
