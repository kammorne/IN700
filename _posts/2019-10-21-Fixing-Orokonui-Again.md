---
layout: post
title: "Fixing Orokonui Again"
date: 2019-10-21
category: Project
tags: project web-development orkonui webapp jekyll
---

# Fixing Orokonui Again

Today I went through the orokonui web app that was running on the live Docker container, and soon found out that it wasn't running the up-to-date version of the files which had the SQL implementation, so I initiated a merge request for the branch I was working on
on my local machine, and once that was merged, I began work on getting the files onto the live server. I thought it would be a simple git pull, however once I did that, the live site broke, and wouldn't show the map. I consulted Josh, since he knew about how the
docker container worked, and he let me know that it may be because the container hasn't been updated, so he taught me about the 'docker-compose build' and 'docker-compose up' commands. So I ran those two commands, checked the server, and found that it fully broke the
web app and brought it down to an "Internal Server Error".

Looking at the logs of the docker container, we soon found that it wasn't importing the required files, and it wasn't accessing the .ENV file that we installed for security. After some tinkering with files and adding the .ENV file to the container, we got the webapp
running on the new files, however it wouldn't load the map still, I went to check the other pages to see if those worked, which they did, but then once we went back to the map page, the map loaded and showed the correct information.

After we made sure the map was fully working, I went on to update the Documentation for the web app to include the information for the docker container, and a better way to install the requirements for a local machine.
