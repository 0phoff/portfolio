---
layout: page
title: Brambox
description: Python library for managing annotations and computing detection statistics
meta: >
    <a href="https://gitlab.com/eavise/brambox" target="_blank">Code</a> - 
    <a href="https://eavise.gitlab.io/brambox" target="_blank">Documentation</a>
img: assets/img/brambox.png
imgclass: pad
importance: 1
category: code
---

While working on object detection problems, I encountered a lot of different formats for storing both annotations and detection results.
Instead of rewriting the parsing logic for each project, I decided to build a dedicated library together with some research colleagues from EAVISE.

Brambox, or _"Basic Requisites for Algorithms on iMages toolBOX"_, is a python library that enables a user to easily load and save different object detection formats.
It is build on top of the well-known pandas library, giving researchers lots of possibilities for extending it and using it with other libraries.
Over time, we have added a lot of extra features, providing extensively tested implementations for most of the different object detection and tracking statistics.  

Brambox has been developed with many development good practices in mind and as such follows semantic versioning, has unit tests covering more than 90% of the library and is fully documented.