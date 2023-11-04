---
layout: page
title: Vansteelandt
description: Automatic metadata extraction from aerial imagery
meta: 2020 - 2022
img: assets/img/vansteelandt.png
imgclass: contain pad
importance: 1
category: phd
related_publications: ophoff_plane
---

Vansteelandt is a geo-surveying company which flies over Flanders on a yearly basis, capturing high resolution aerial imagery.
Looking for a way to further exploit this data, they started a project with the EAVISE research group in order to develop AI algorithms, capable of extracting various metadata from the images.

Building on my previous experience with satellite imagery, I firstly developed a pipeline to be able to train and run deep learning models on these aerial images, automatically handling the division of the images in smaller the chunks, whilst keeping the possibility to transform the output of the models to proper geographical coordinates.
This enabled various researchers to develop a plethora of AI models, capable of extracting different metadata from the aerial footage.
Finally, I used this pipeline to research the potential of object detection on this high resolution data. More specifically, I developed and trained convolutional neural networks capable of detecting solar panels and swimming pools.
Furthermore, I designed a methodology to fuse RGB and depth data, increasing the accuracy of the detection models.