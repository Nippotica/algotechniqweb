---
layout: page
title: DeepHole
description: Real-time road quality detection on Edge
img: assets/img/deephole.webp
importance: 2
category: work
related_publications: true
---



### Objective
The new goal of this project is to implement a real-time road quality inspection system using AI-on-the-Edge technologies, specifically deploying deep learning models on edge devices like the Nvidia Jetson Nano. This approach aims to enhance the efficiency and accuracy of pothole detection, making it more feasible for real-time applications.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/deephole.webp" title="DeepHole Algotechniq" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Potholes make roads unsafe.
</div>

### Prior Work
Previously, pothole detection was achieved through various methods including manual inspections, sensor-based systems, 3D reconstruction, and traditional computer vision techniques {% cite 10.1145/1378600.1378605 %}{% cite abou2018municipal %}. However, these methods faced challenges such as being time-consuming, costly, weather-dependent, and requiring expensive hardware. Traditional computer vision techniques also suffered from false detections and were less effective in varying road conditions {% cite vehicles5030051 %}.

### Benefits
The new approach will benefit road maintenance authorities by providing a faster and more accurate system for detecting and responding to potholes. Additionally, it can be advantageous for self-driving applications, the automation industry, and possibly public safety sectors by improving road condition assessments and reducing the risk of accidents.

### Enabling Technologies
The key enabling technologies of the new approach include deep learning models (specifically YOLO family models like YOLOv8), AI-on-the-Edge implementation using the  Nvidia Jetson Nano as the edge computing platform. The system also leverages the Nvidia TensorRT for model deployment on edge devices.

### Measuring Performance
The success of the new approach can be quantified through various performance metrics such as mean average precision (mAP), detection accuracy, frames per second (FPS), and inference time. 