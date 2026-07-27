---
layout: page
title: 无人机编队鲁棒控制
description: 面向突发飞行事件的消费级无人机编队可靠性增强
img: assets/img/projects/uav-formation-control-title.png
importance: 1
category: work
---

## 项目概述

本项目研究消费级无人机在突发飞行事件下的可靠编队控制问题。针对风扰动补偿滞后、固定通信拓扑可能放大局部性能退化等挑战，构建了融合**预设性能控制**、**预设时间扰动观测器**与**自适应加权邻接矩阵**的协同控制框架。

项目对应论文：*Enhancing Consumer UAV Formation Reliability Under Unexpected In-Flight Contingencies: Prescribed Performance Control With an Adaptive Weighted Adjacency Matrix*。

参与成员：Qi Yang、Yongze Li、**Ban Wang**（通讯作者）。

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/uav-formation-control-abstract.png" title="项目摘要" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

## 核心特点

- 将包含邻居信息的编队误差引入预设性能约束，实现误差有界收敛。
- 采用与性能函数共享预设时间参数的扰动观测器，同时保障暂态与稳态误差调节。
- 根据无人机跟踪误差在线调整邻接权重，减弱局部性能退化成员的协同影响，抑制误差在拓扑中的传播。
- 通过仿真与实机实验验证控制器在风扰动及突发飞行事件下的收敛速度和恢复能力。

## 实验视频

### 视频 1：控制器有效性实机验证

<video class="img-fluid rounded z-depth-1" controls preload="metadata">
  <source src="https://yangqi-npu.github.io/UAV-Formation-Control-Project/videos/controller_effectiveness.mp4" type="video/mp4">
  您的浏览器不支持视频播放。
</video>

### 视频 2：风扰动下的扰动观测器验证实验

<video class="img-fluid rounded z-depth-1" controls preload="metadata">
  <source src="https://yangqi-npu.github.io/UAV-Formation-Control-Project/videos/disturbance_observer.mp4" type="video/mp4">
  您的浏览器不支持视频播放。
</video>

项目原始页面：[查看完整项目介绍与实验视频](https://yangqi-npu.github.io/UAV-Formation-Control-Project/)。
