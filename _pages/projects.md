---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /resume
---
Here are all the projects I done before by myself or collaborate with others, feel free to explore!

- [Crowd-sourced Mapping](#cloud-based-crowd-sourced-mapping-for-mass-produced-models)
- [Hybrid A* Application](#hybrid-a-application-in-intersections-u-turn-line-generation)
- [UGV Robot Experiments](#ugv-robot-experiments)
- [Jump Point Search](#jump-point-search-algorithm)
- [Dynamic Programming](#dynamic-programming)
- [CEC Control](#cec-control)

## Cloud-based Crowd-sourced Mapping for Mass-produced Models
In the field of autonomous driving mapping, in addition to the traditional high-precision (HD) maps and real-time mapping that relies entirely on perception, a mainstream method is crowd-sourced mapping. By uploading the perception results of the vehicle side, multiple trips and a large amount of data are collected in the cloud for automatic aggregation to achieve a crowd-sourced map with high accuracy, low cost, and high freshness. Crowd-sourced maps can well assist downstream planning and control modules in autonomous driving.

Our solution leverages the MapTR V2 model as a baseline for improvement. This trained model is adept at identifying ground elements, such as lane markings. Within the cloud module, my responsibilities include developing the incremental fitting module with multi-frame perception, the matching module of perception map and base maps, the variation detection module, and the automatic fusion module. Each of these modules plays a crucial role in our solution, contributing to its overall effectiveness.

Among them, I designed a complete set of map evaluation and fusion system based on base map matching. This system can segment the new perception results based on the historical information of the base map and calculate the absolute mean error (MAE) and the mean relative error (MRE) of the lines to measure the perception quality. The detection result will be used as the input of map fusion, vital in determining the fusion confidence. 

<figure>
  <img src="/images/vector map/map updating pipeline png ver.png" width=800px/>
  <center>
    <figcaption>map evaluation and fusion system pipeline</figcaption>
   </center> 
</figure>

The variation results shown above are obtained from real experiments in Guangzhou's downtown. The scenario shows a complicated intersection mixing highway and city road. The right-hand side result is the fusion result achieved by automatic fusion and manual validation.

Our work in perception model (Received by WACV 2025)
-  [PrevPredMap: Exploring Temporal Modeling with Previous Predictions for Online Vectorized HD Map Construction](https://arxiv.org/abs/2407.17378)
- my contributions involves in whole training data support and map vector result post-process


## Hybrid A* Application in Intersection's U-turn Line Generation

Autonomous vehicles face challenges navigating complex urban roads, particularly at intersections. The virtual line, e.g. the u-trun lines are used to represent the topology geometry assisting the downstream planning and control. The virtual lines in map usually have the strtic curvature requirement which the traditional curve generator cannot guareteen. This study novetlty proposes an approach using a search-based planning algorithm in curve generation. The main features are:

1) The vehicle kinematic model uses constant speed and continuous integration to express the state transfer equation.
2) The generated curve's global maximum curvature is guaranteed.
3) Adaptive curve smooth parameters mechanism for lane scenario variation

|Animation|Ackermann-Drive Kinematic Model|U-turn Scenario|
|-|-|-|
|<img src="/files/HybridAstar_gif1.gif" width=330px/>|<img src="/images/planning/ackermann.png" width=330px>|<img src="/images/planning/uturn_scene.png" width=330px>|

In our experiments, a maximum curvature of 0.1740 is the best among the four methods, and the curvature pass rate is greatly improved to 81.48%. In terms of the maximum curvature change and the maximum curvature change $\sigma$, both are improved from the plain version. It is proved that our method can improve the curvature pass rate while maintaining a certain degree of smoothness, meeting the requirements of curvature and smoothness.

<figure>
  <img src="/images/planning/curvature_table.png" width=1000px/>
  <center>
    <figcaption>statistic results with the experiments in 30 urban intersections</figcaption>
  </center>
</figure>

## Jump Point Search Algorithm
A 2D target chasing problem solving by JPS algorithm

## UGV Robot Experiments

|Real-time Manipulation in Rviz Visualization||
|-|-|
|Hector Mapping|Frontier-based Exploration|
|<img src="/images/ERL/hector_gif.gif" width=500px/>|<img src="/images/ERL/Frontier_gif.gif" width=500px/>|
|LIMO-3D SLAM with Ouster1-32|LIMO-3D SLAM with Ouster1-32|
|<img src="/images/ERL/Limo3D_gif.gif" width=500px/>|<img src="/images/ERL/Limo3D_pic.png" width=500px/>|
|TARE Planner in Jackal|iSDDF Planner in Jackal|
|<img src="/images/ERL/TARE_gif.gif" width=500px/>|<img src="/images/ERL/SDDF_gif.gif" width=500px/>|

<!-- |<img src="/files/fusion_gif1-1.gif" width=600px/>|
|<img src="/images/vector map/Fusion_error_gif.gif" width=600px/>| --> 

<!-- ## Object Detection -->
<!-- ### Bin Detector with Bayes Filter
A vision object detection task to find the blue bin in the pictures

|Detection Box|Mask|
|-|-|
|<img src="/images/vision/0061_box.png" width=400px/>|<img src="/images/vision/0061_mask.png" width=400px/>|
|<img src="/images/vision/0065_box.png" width=400px/>|<img src="/images/vision/0065_mask.png" width=400px/>|
|<img src="/images/vision/0067_box.png" width=400px/>|<img src="/images/vision/0067_mask.png" width=400px/>| -->
<!-- 
### Phone Detector with SVM
A vision object detection task to find the phone in the pictures

|Phone1|Phone2|
|-|-|
|<img src="/images/vision/phone1.png" width=400px/>|<img src="/images/vision/phone2.png" width=400px/>| -->

## Dynamic Programming
A 2D Door-Key problem solved by dynamic programming, aims to find the optimal policy.

|Single Door Scenario|Two Doors Scenario|
|-|-|
|<img src="/images/planning/doorkey1.gif" width=400px/>|<img src="/images/planning/doorkey3.gif" width=400px/>|
|<img src="/images/planning/doorkey2.gif" width=400px/>|<img src="/images/planning/doorkey4.gif" width=400px/>|


## CEC Control

|Free Space|Collision Aware|
|-|-|
|<img src="/images/planning/CECfree.gif" width=400px/>|<img src="/images/planning/CEC1.gif" width=400px/>|

<!-- ## Optimal Scene Graph Planning with Large Language Model Guidance
<img src="/images/planning/room_door_toplogy.png" width=800px/> -->

