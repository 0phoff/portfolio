---
layout: page
title: OmniDrone
description: Autonomous drones with 720⁰ perceptual vision
meta: 2017 - 2019
img: assets/img/omnidrone.png
imgclass: contain pad
importance: 1
category: phd
related_publications: ophoff_rgbd01, ophoff_rgbd02, ophoff_speed, ophoff_erti
---

The OmniDrone project researched unmanned areal vehicles and the important challenges to overcome regarding the drone’s reliability and use.
It therefore focussed on the increase of a drone's intelligence and awareness of its environment, using 720-degree stereo omnidirectional camera systems.
The main technological objectives of OmniDrone were therefore to enable real-time, on board, 720 degree cognitive vision and to exploit it towards ultra-reliable operation and pilot-assist, giving drones increased reliability and ease-of-use within security and surveillance, professional video broadcast, inspection and traffic monitoring.

Within this project, it was my task to enable fast and reliable object detection on-board the drone, using an embedded Jetson TX2 platform.
Firstly, I investigated the potential gains of fusing RGB and depth data in order to increase the detection accuracy.
I developed a model capable of running on both inputs in parallel, eventually fusing both streams at an parametrizable point in the network.
Extensive experimentation then demonstrated that fusing both streams towards the end of the network yields the best results, effectively surpassing both RGB- and depth-only models.

Afterwards, I researched how to best combine a variety of speed optimisation techniques for convolutional neural networks, in order to achieve real-time detection on the device.
The outcome of this research was a model that ran 15 times faster than the original, meanwhile even increasing the accuracy on an industrial dataset.