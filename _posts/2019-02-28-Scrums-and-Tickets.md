---
layout: post
title: "Scrums and Tickets"
date: 2019-02-28
category: Project
tags: project nodes web-development jekyll
---

# Scrums and Tickets

We had our first scrum as a team today, and we discussed certain tickets and how the team was going to get through with it. I ended up being assigned to creating a
website for Linus, one of our clients, that would display the information being sent from the temperature sensors we created in the previous class. After doing a bit
of research and talking to the other members of the team who were here last semester, I found out the devices used an MQTT broadcast to send the data. Unfortunately, none
of the team knew more than that, so I talked to Tom and asked if he could provide some information about how the devices actually send information. He provided a rough but
understandable diagram of how the nodes sent information through the gateway to the LoRa server, and then how it was sent through the MQTT Broadcast, before being saved in a
database. With that in mind, I began working on the website for Linus.
