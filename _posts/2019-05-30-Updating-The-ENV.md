---
layout: post
title: "Updating the ENV"
date: 2019-05-30
category: Project
tags: project web-development iotdata webapp server ENV jekyll
---

# Updating the ENV

Today I've been trying different things regarding the database webapp, and tinkered a bit with using the Google Authentication, however I didn't
really get anywhere with that, since it kept throwing errors, so I scrapped what I had for now, and looked at other ways I could optimize the webapp.

While looking through the files, I found out that the config I had written for the ENV file wasn't even being used, since it was for a different
version of the dotENV files, designed more for exclusively Flask applications, where I'm currently using a more broader python dotENV package.

I also looked at ways I could remove more sensitive information for the webapp, and changed the application's port and host to be loaded through
the ENV file instead of having plaintext information on the app.py file.
By doing this, it allows other modules to use these variables later without code duplication.
