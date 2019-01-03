---
layout: inner
position: left
title: 'CeilingBot'
date: 2018-12-12 16:45:00
categories: development
tags: ROS OpenCV RaspberryPi Arduino
featured_image: '/img/posts/04_ceilingbot.jpg'
project_link: ''
button_icon: ''
button_text: ''
lead_text: 'Building localization, no RF or LIDAR required'
---

The idea of CeilingBot started with a senior project idea that never got off the ground: A robot that could navigate a large, crowded building, such as a hospital or an airport, and do it on a budget.  We quickly rejected SLAM as our only means of localization - after all, depending on occupancy conditions a 2-D scan LIDAR might not even be able to see the walls.  We also considered RF localization, but discarded the idea due to worries about reflection in an indoors environment.

Our solution was simple: while the robot may not be able to see the walls around it, it can always see the ceiling.  Thus, localization is possible with nothing more than an upwards-facing camera and a set of reference markers on the ceiling.

While the project never got off the ground due to the loss of a team member, I am now attempting to implement only the ceiling localization part of the planned robot on a small, cheap platform.  This lets me test the functionality of my idea while teaching myself ROS and OpenCV at the same time.
