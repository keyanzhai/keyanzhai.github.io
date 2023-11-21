---
title: Scaffolded Learning of In-place Trotting Gait for a Quadruped Robot with Bayesian Optimization
date: 2020-11-19 19:10:21
academia: true
---

**Publication** [[**Springer**](https://link.springer.com/chapter/10.1007/978-3-030-95892-3_28)][[**arXiv**](https://arxiv.org/abs/2101.09961)][[**code**](https://github.com/keyanzhai/Slimdog)][[**slides**](https://1drv.ms/p/s!AuXcCtfGaQlXg7QnW-4KvFFFTjsgGg?e=eXJ6RU)]: 
Keyan Zhai, Chu'an Li, and Andre Rosendo. "Scaffolded Learning of In-place Trotting Gait for a Quadruped Robot with Bayesian Optimization." 16th International Conference on Intelligent Autonomous Systems ([IAS-16](https://www.ias-16.com/)).

**Abstract**
During learning trials, systems are exposed to different failure conditions which may break robotic parts before a safe behavior is discovered. Humans contour this problem by grounding their learning to a safer structure/control first and gradually increasing its difficulty. This paper presents the impact of a similar supports in the learning of a stable gait on a quadruped robot. Based on the psychological theory of instructional scaffolding, we provide different support settings to our robot, evaluated with strain gauges, and use Bayesian Optimization to conduct a parametric search towards a stable Raibert controller. We perform several experiments to measure the relation between constant supports and gradually reduced supports during gait learning, and our results show that a gradually reduced support is capable of creating a more stable gait than a support at a fixed height. Although gaps between simulation and reality can lead robots to catastrophic failures, our proposed method combines speed and safety when learning a new behavior.

## Motivation

<p align="center"><video style="width:100%" controls>
<source src="resources/failures.mp4"></video></p>

## Experiments

<figure>
  <img src="resources/Slimdog1.JPG" alt="Slimdog" style="width:100%">
  <figcaption>Fig.1 - The Slimdog robot</figcaption>
</figure>

<figure>
  <img src="resources/Comparison_min_red_no.png" alt="Comparison of no support, minimum support and reducing support" style="width:100%">
  <figcaption>Fig.2 - Comparison of no support, minimum support and reducing support</figcaption>
</figure>

## Kinovea Analysis

### No support (No_P1, 1st run, fitness = 72.83)

<p align="center"><video style="width:100%" controls>
<source src="resources/No_P1_R1_Kinovea3.mp4"></video></p>

### Minimum support (Min_P1, 1st run, fitness = 72.43)

<p align="center"><video style="width:100%" controls>
<source src="resources/Min_P1_R1_Kinovea3.mp4"></video></p>

### Reducing support (Red_P1, 3rd run, fitness = 75.92)

<p align="center"><video style="width:100%" controls>
<source src="resources/Red_P1_R3_Kinovea3.mp4"></video></p>


## Results

### Knee and joint angles

<figure>
  <img src="resources/Comparison_Joint_Angles.jpg" alt="Knee and joint angles" style="width:100%">
  <figcaption>Fig.3 - Knee and joint angles</figcaption>
</figure>

### Vertical translation of center of mass

<figure>
  <img src="resources/Comparison_Body_V_Pos_new.jpg" alt="Vertical translation of center of mass" style="width:100%">
  <figcaption>Fig.4 - Vertical translation of center of mass</figcaption>
</figure>
