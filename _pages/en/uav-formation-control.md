---
layout: lab-en
permalink: /en/projects/uav_formation_control/
translation: /projects/uav_formation_control/
title: Robust Control for UAV Formations
description: Improving the reliability of consumer UAV formations during unexpected in-flight events.
img: assets/img/projects/uav-formation-control-title.png
lab_nav_parent: /en/projects/
---

## Project Overview

This project studies how consumer UAVs can maintain reliable formations during unexpected in-flight events. Delays in compensating for wind disturbances and fixed communication topologies can allow a local loss of performance to spread through a formation. The proposed cooperative controller combines **prescribed performance control**, a **prescribed-time disturbance observer**, and an **adaptive weighted adjacency matrix**.

Related publication: *Enhancing Consumer UAV Formation Reliability Under Unexpected In-Flight Contingencies: Prescribed Performance Control With an Adaptive Weighted Adjacency Matrix*.

Project contributors: Qi Yang, Yongze Li, and **Ban Wang** (corresponding author).

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/uav-formation-control-abstract.png" title="Project overview" alt="Overview of the UAV formation control project" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

## Approach and Validation

- Incorporate neighboring aircraft into the formation error and use prescribed performance constraints to keep the error bounded as it converges.
- Use a disturbance observer with the same prescribed-time parameter as the performance function to regulate transient and steady-state errors.
- Adjust adjacency weights online based on tracking error to reduce how much a poorly tracking aircraft affects its neighbors and limit error propagation.
- Use simulations and flight tests to evaluate convergence speed and recovery under wind disturbances and unexpected in-flight events.

## Flight Test Videos

### Controller effectiveness

<video class="img-fluid rounded z-depth-1" controls preload="metadata">
  <source src="https://yangqi-npu.github.io/UAV-Formation-Control-Project/videos/controller_effectiveness.mp4" type="video/mp4">
  <a href="https://yangqi-npu.github.io/UAV-Formation-Control-Project/videos/controller_effectiveness.mp4">Open the controller effectiveness video</a>
</video>

### Disturbance observer under wind

<video class="img-fluid rounded z-depth-1" controls preload="metadata">
  <source src="https://yangqi-npu.github.io/UAV-Formation-Control-Project/videos/disturbance_observer.mp4" type="video/mp4">
  <a href="https://yangqi-npu.github.io/UAV-Formation-Control-Project/videos/disturbance_observer.mp4">Open the disturbance observer video</a>
</video>

[Full project description and flight test videos](https://yangqi-npu.github.io/UAV-Formation-Control-Project/)
