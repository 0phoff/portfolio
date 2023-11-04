---
layout: page
title: Lightnet
description: PyTorch Library with a focus on single-shot object detection
meta: >
    <a href="https://gitlab.com/eavise/lightnet" target="_blank">Code</a> - 
    <a href="https://eavise.gitlab.io/lightnet" target="_blank">Documentation</a>
img: assets/img/lightnet.png
imgclass: pad
importance: 1
category: code
---

During my PhD, I developed a plethora of detection models, each with their pros & cons.
All of these models, together with their necessary loss, pre- and post-processing have been implemented in a single PyTorch library, called Lightnet.

The main goal of this library was to create a modular set of building blocks, allowing you to easily integrate these models into various different applications.
As such it is fairly bare bones and only provides a set of `torch.nn.Modules`, which a user can utilize to scaffold out an entire pipeline.  
I took this approach even further by also constructing the various models out of different modules, allowing for rapid prototyping and development of new models.