---
title: "Shepherding with Deep Reinforcement Learning"
collection: publications
permalink: /publication/Shepherding with Deep Reinforcement Learning
excerpt: 'This paper is about learning a robust group controller using deep reinforcement learning .'
date: 2021-03-25
venue: 'IEEE Robotics and Automation Letters'
paperurl: 'https://ieeexplore.ieee.org/document/9387150/'
citation: 'Jixuan Zhi, and Jyh-Ming Lien. "Learning to herd agents amongst obstacles: Training robust shepherding behaviors using deep reinforcement learning." IEEE Robotics and Automation Letters 6, no. 2 (2021): 4163-4168.'
---
Overview

The robotic shepherding problem considers the control and navigation of a group of coherent agents (e.g., a flock of birds or a fleet of drones) through the motion of an external robot, called a shepherd. However, the existing method shows that shepherding robots cannot robustly herd agents amongst obstacles under uncertain behavioral and environmental models.

We propose the first known learning-based method that can herd agents amongst obstacles. By using deep reinforcement learning techniques combined with the probabilistic roadmaps, we train a shepherding model using noisy but controlled environmental and behavioral parameters.

We consider a partially-observable continuous world, in which the shepherd robot can only observe the state of the world in a field of view centered around itself. We choose to represent the group as a bounding circle as shown in the figure and define the position of the sheep as the center of the group. To handle environments populated with obstacles, a path planner will inquire the probabilistic roadmaps (PRM) and find a steering path as a sub-goal to connect the sheep (center) to the goal.

We consider the environments with predefined obstacles. In practice, the environment (such as in a farm or ranch) is usually fixed, and the sheep routinely move toward one location for grazing and the other location for drinking. Therefore, we create a fixed environment as follows. We set two positions and alternate between these two positions as the start and goal. The figure shows two trajectories in opposite directions that successfully herd a group of three sheep in the filter environments.

We train the controller in environments with randomly perturbed obstacles. The figure as follows shows two examples composed of fences that partition the spaces into long corridors with narrow gaps and sharp turns. To train the controller, we create three-layer obstacle environments (left) and perturb the position and angle of each fence using a clipped Gaussian noise. For the gaps formed by two fences, the shorter fence may appear or disappear randomly thus changing the difficulty of the herding problem.

To evaluate the trained model, we build a set of similar but more difficult environments containing four layers with one to four gaps is shown as follows, the figure also illustrates the successful herding paths and a side-to-side steering policy by learning.

[paper](https://ieeexplore.ieee.org/document/9387150/)

