---
title: "Visibility Integrity Region"
collection: publications
permalink: /publication/VisibilityIntegrityRegion
excerpt: 'This paper is about the group following problem in 3D with visibility integrity.'
date: 2019-07-25
venue: 'IEEE Robotics and Automation Letters'
paperurl: 'https://ieeexplore.ieee.org/document/8772150/'
citation: 'Jixuan Zhi, Yue Hao, Christopher Vo, Marco Morales, and Jyh-Ming Lien. "Computing 3-d from-region visibility using visibility integrity." IEEE Robotics and Automation Letters 4, no. 4 (2019): 4286-4291.'
---
**Abstract**  
Visibility integrity (VI) is a measurement of similarity between the visibilities of regions. We present a method that speeds up VI computation from O(n^4logn) to O(n^2) and introduce the visibility-integrity roadmap (VIR), a data structure for 3-D group visibility and planning. We demonstrate applications in group tracking, such as camera motion planning to maintain visibility of moving targets in 3-D environments.

**Layman’s Summary**  
Imagine a camera tracking a swarm of drones in a cluttered 3D space. Our method helps the camera ‘lazily’ follow the group by precomputing visibility zones (VIRs) offline. This reduces computation time drastically and ensures the camera moves efficiently while keeping most targets in view.

**Key Visuals**

+ **Figures to Highlight:**
  + Figure 1: Visibility integrity values (high vs. low).
  + Figure 2: Visibility-integrity regions in 3D environments (grid-based vs. kernel-based)
  + Figure 4: Simulation environments (tower, pachinko, ruins, canyon).

**Infographics**: Summarize the VI workflow (sampling → clustering → VIR construction → planning).

**Significance & Impact**
+ **Key Contributions:**

  + Reduces VI computation time from O(n^4logn) to O(n^2)
  + First offline method to compute VIRs in 3D for real-time group tracking.
  + "Lazy" camera motion: 50–80% less movement than baseline methods.

+ **Applications:** Robotics, UAV surveillance, deformable/articulated object tracking.

[paper](https://ieeexplore.ieee.org/document/8772150/)



