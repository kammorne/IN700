---
layout: post
title: "Fixing The Heatmap"
date: 2019-10-14
category: Project
tags: project web-development heatmap webapp jekyll
---

# Fixing the Heatmap

After our small break over the holidays, we returned ready to begin on a new sprint. Martin greeted us, and let us know that the heatmap webapp wasn't reading data, and hasn't for nearly a month (late September) I figured that it was
related to when we changed over to The Things Network, and offered to take on the task of fixing the issue. Josh also offered to give me a hand, since he wanted to have a closer look at the webapp, since he was going to be installing
the webapp onto the Docker Server once it was done.

After looking into the VM for the heatmap, I soon figured out that it was as I suspected, and that the code was calling from the old LoRa network MQTT Broadcasts, so it wasn't able to update the information. Luckily, Henry had already updated
the code to work with The Things Network, so I thought it would be an easy task of doing a 'git pull' in the repository the app was saved in. However, it wasn't that easy, as we soon found out that the webapp was saved in someone's private repository,
and it wasn't giving us access because of that. Henry also let me know that the app was being hosted via a 'screen' command, rather than a service or even as an apache service. I knew this wouldn't work in the long run, and ended up looking into
hosting the app properly, however it soon became quite a task where I had to jump through a lot of hoops to get it working. In the end, I didn't even get it running, and began looking into getting the app running on apache, since it looked like the app's
backend was run on Django.

Josh and I ended up getting an Apache server running, however the server wouldn't accept the Django files. In the end, I was both getting frustrated and had to leave to get to an appointment, so I decided to leave it and come back once I had a level head.
