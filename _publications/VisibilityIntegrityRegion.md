---
title: "Visibility Integrity Region"
collection: publications
permalink: /publication/VisibilityIntegrityRegion
excerpt: 'This paper is group following problem in 3D with visibility integrity.'
date: 2019-07-25
venue: 'IEEE Robotics and Automation Letters'
paperurl: 'https://ieeexplore.ieee.org/document/8772150/'
citation: 'Jixuan Zhi, Yue Hao, Christopher Vo, Marco Morales, and Jyh-Ming Lien. "Computing 3-d from-region visibility using visibility integrity." IEEE Robotics and Automation Letters 4, no. 4 (2019): 4286-4291.'
---
Overview

Computing from-region visibility is a fundamental problem that involves determining the visible part of a 2D or 3D space from a given region. It is not well studied if regions are moving such as moving crowds.

We propose an idea called Visibility integrity, which is used for measuring the similarity between the visibilities of regions. We draw samples and compute point-to-point visibilities to approximate the from-region visibility of moving regions, called group visibility.

Based on the new idea of visibility integrity, we show that the visibility-integrity roadmap, a data structure that partitions space into zones, can be used to solve group visibility and the group following problems in 3D.

The group following problem involves finding a sequence of positions and orientations of the camera to maximize the number of visible targets during a specified period of time. To find the position of the camera, we first predict the target position, then assign the position to a visibility integrity region, and finally predict and evaluate camera positions by querying the visibility-integrity roadmap.



[paper](https://ieeexplore.ieee.org/document/8772150/)



