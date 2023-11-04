---
layout: page
title: SatCen
description: Automatic monitoring of vehicles and vessels in satellite imagery
meta: 2019 - 2020
img: assets/img/satcen.png
imgclass: contain pad
importance: 1
category: phd
related_publications: ophoff_satellite
---

Since 2013, The EU Satellite Centre (SatCen) delivers services and information products for border surveillance to the European Border and Coast Guard Agency, Frontex.
This requires continuous improvement of services and capturing new developments in the market in order to eventually introduce them in operations.
A daily concern in the Operations Division is dealing with large datasets of very high resolution images, looking for small objects that may be related to illegal migration or cross-border crime.
SatCen thus wanted to investigate the potential of AI to help analysts monitor vehicle and vessels in these high resolution satellite images.

Within this project, I developed a pipeline to be able to run deep learning models on this data, automatically dividing these orthomosaic images in smaller chunks with overlap between, in order to deal with objects that lie on the border between different chunks.
Using this pipeline, I then evaluated a variety of different single shot detection models for the specific case of vehicle and vessel detection.
