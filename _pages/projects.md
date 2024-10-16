---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /resume
---
Here are all the projects I have done before or collaborated with others; feel free to explore!

- [Crowd-Sourced Map Updating](#crowd-sourced-map-updating)
- [Hybrid A* Planner](#hybrid-astar-planner)
- [Jump Point Search](#jump-point-search-algorithm)
- [UGV Robot Real-time and Simulation ](#ugv-robot-experiments)
- [Dynamic Programming](#dynamic-programming)
- [CEC Control](#cec-control)
- [Object Detection](#object-detection)

<!-- - [LLM Planning](#optimal-scene-graph-planning-with-large-language-model-guidance) -->

## Crowd-Sourced Map Updating
In autonomous driving, especially in complex urban areas, high-precision (HD map) maps play a vital role. In contrast, HD maps have the problems of high production costs and untimely updates. Therefore, in recent years, multi-source light maps have received much attention in the industry. We have improved the MapTR V2 model and used it to generate BEV perception vector maps. The module I am responsible for combines the results of multi-trip perception with the crowd-sourced base map and performs variation detection, fusion, and update. 

The pipeline is under below: 

<img src="/images/map updating pipeline png ver.png" width=1000px/>

## Hybrid Astar Planner
Generating a driveable U-turn curve with precise curvature constraints while ensuring the vehicle remains within
lane boundaries is crucial for safety. This study proposes an approach using a search-based planning algorithm combined with a non-holonomic vehicle motion model. Hybridizing the Ackermann-drive motion model into the A* planner’s expansion step enables the retention of optimality and ensures safety and comfort constraints.

|Animation|Ackermann-Drive Kinematic Model|
|-|-|
|<img src="/files/HybridAstar_gif1.gif" width=300px/>|<img src="/images/planning/ackermann.png" width=600px>|

## Jump Point Search Algorithm
A 2D target chasing problem solving by JPS algorithm

## UGV Robot Experiments
|||
|-|-|
|Hector Mapping|Frontier-based Exploration|
|<img src="/images/ERL/hector_gif.gif" width=500px/>|<img src="/images/ERL/Frontier_gif.gif" width=500px/>|
|LIMO-3D SLAM with Ouster1-32|LIMO-3D SLAM with Ouster1-32|
|<img src="/images/ERL/Limo3D_gif.gif" width=500px/>|<img src="/images/ERL/Limo3D_pic.png" width=500px/>|
|TARE Planner in Jackal|iSDDF Planner in Jackal|
|<img src="/images/ERL/TARE_gif.gif" width=500px/>|<img src="/images/ERL/SDDF_gif.gif" width=500px/>|

<!-- |<img src="/files/fusion_gif1-1.gif" width=600px/>|
|<img src="/images/vector map/Fusion_error_gif.gif" width=600px/>| --> 

## Object Detection
<!-- ### Bin Detector with Bayes Filter
A vision object detection task to find the blue bin in the pictures

|Detection Box|Mask|
|-|-|
|<img src="/images/vision/0061_box.png" width=300px/>|<img src="/images/vision/0061_mask.png" width=300px/>|
|<img src="/images/vision/0065_box.png" width=300px/>|<img src="/images/vision/0065_mask.png" width=300px/>|
|<img src="/images/vision/0067_box.png" width=300px/>|<img src="/images/vision/0067_mask.png" width=300px/>| -->

### Phone Detector with SVM
A vision object detection task to find the phone in the pictures

|Phone1|Phone2|
|-|-|
|<img src="/images/vision/phone1.png" width=400px/>|<img src="/images/vision/phone2.png" width=400px/>|

## Dynamic Programming
A 2D Door-Key problem solved by dynamic programming, aims to find the optimal policy.

|Single Door Scenario|Two Doors Scenario|
|-|-|
|<img src="/images/planning/doorkey1.gif" width=300px/>|<img src="/images/planning/doorkey3.gif" width=300px/>|
|<img src="/images/planning/doorkey2.gif" width=300px/>|<img src="/images/planning/doorkey4.gif" width=300px/>|

## CEC Control

|Free Space|Collision Aware|
|-|-|
|<img src="/images/planning/CECfree.gif" width=300px/>|<img src="/images/planning/CEC1.gif" width=300px/>|

<!-- ## Optimal Scene Graph Planning with Large Language Model Guidance
<img src="/images/planning/room_door_toplogy.png" width=800px/> -->

