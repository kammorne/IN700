---
layout: post
title: "Fixing Broken CO2 Board"
date: 2019-11-07
category: Classwork
tags: classwork project thingsnetwork co2sensor jekyll
---

# Fixing Broken CO2 Board

So Bee came to me today and let me know that the first board, CO2_01, had a dead sensor, which is why it was giving the 16ppm reading all the time.
Luckily, we had another sensor free, since we originally planned on having 4 sensors, although we unfortunately did not have enough Adafruit
boards to be able to do that, so we took the sensor for the 4th board, and used it to replace the broken sensor on CO2_01. Luckily, we only
hot-glued the sensor to the board, although I thought that may have been what caused the issue in the first place, although it hasn't affected
any of the other boards so far.

![CO2 Fix 1](https://kammorne.github.io/lagoma1_IN700/img/CO2Replace.jpg)
![CO2 Fix 2](https://kammorne.github.io/lagoma1_IN700/img/friedCO2.jpg)

After that was sorted, I ended up soldering the final board we were going to use. This one ended up being more of an issue, since it wouldn't compile,
and when plugged into the computer, it would throw a Power Surge error, and then the computer wouldn't pick it up. After looking through all the solder
points, and adjusting them where the tiniest bridging had occurred, we finally got the sketch uploaded onto the board, and it started sending data without
issue.
