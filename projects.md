---
layout: default
title: Projects
permalink: /projects/
---

## Overview
 - Bachelor thesis, Sleep scoring with Keras
 - Crazyfly drone project
 - RuneLite development

## Sleep scoring with Keras
For my bachelor thesis I created a dense network classifier in python with keras. The goal was to use EEG and EMG data to analyze sleeping patterns for rats, also called sleep scoring. This process is currently done manually and the results would greatly reduce the time that researchers have to spend doing this tideous task. I used a preprocessing technique called feature extraction where some relevant statistical features were extracted from the data and then fed through the neural network.

![EEG features](/assets/bachelor_eeg_plot.png)

The resulting neural network had an accuracy of a little over 97 %.

Full paper available [here](http://urn.kb.se/resolve?urn=urn:nbn:se:kth:diva-239372) with some code [here](https://github.com/dekvall/rat_sleep_patterns).

## Crazyfly drone project
We implemented a pathfinding, computer vision and localization for a Crazyflie drone for it to be able to fly through a course while recognizing traffic signs for extra points. The only input given was a 3D map so continous localization measures were needed as well as online pathplanning. 

To do the pathfinding we implemented a 2D A\* algorithm on a fixed height. The pathplanning was done in an online fashion.

![pathplanning drone](/assets/robotics_project_path_planning.png)

To do the computer vision we used a convolutional neural network and applied it to every frame with a potential sign in it. 

![traffic signs detected](/assets/robotics_project_traffic_signs.png)

To do the localization we used aruco markers which were placed thorughout the course.

![aruco detected](/assets/robotics_project_aruco.png)

We used these in conjuction with their position on the given map to obtain the drone position through a simplified kalman filter. 

Code not currently publicly available.

## RuneLite development
RuneLite is an open-source 3rd party Old-school Runescape (OSRS) client for which I have written a few enhancements and bug-fixes.

Check out the project [here](https://github.com/runelite/runelite) or my fork [here](https://github.com/dekvall/runelite).



