---
layout: post
title: "Relay Issues"
date: 2019-10-17
category: Project
tags: project web-development heatmap webapp jekyll
---

# Relay Issues

After tinkering with the Heatmap webapp since Monday, Josh and I figured out that the webapp was run on a React build, not a Django build. After figuring this out, and spending some time on Wednesday trying to get the webapp working, We figured we'd just
set up the webapp to run on the Docker container instead of focusing on running it on apache, since we wouldn't even be using it for more than a few weeks while we organized the Docker container. I decided to keep the webapp running on the old janky way
of running it on a 'screen' prompt.

I went to help Josh with getting the webapp running on a Docker container, but soon found out that the app was being finicky with running the 'npm build' command. We spent a while trying to get the app to build the latest version, since the current build
version was running the old MQTT broadcast files. We also found out that the only way to get the MQTT broadcasts to be read by the app was to have a relay running. We also found out that said relay was running on Henry's local machine, which would not work
at all once he leaves, or turns off his machine. So Josh and I decided that we wouldn't bother trying to get the Heatmap running on the Docker container for the moment, but instead focus on getting the relay onto a Docker container, since at least in the current
form, the app will still run on the VM, however once Henry leaves it will be impossible to have the heatmap collect data.
