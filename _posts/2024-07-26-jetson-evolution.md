---
layout: post
title: The Jetson Evolution
date: 2024-07-26 
description: As Nvidia evolves Jetson, embedded systems thrive
tags: technote
categories: Algoblog
---


Nvidia Jetson single-board computers (SBCs) provide versatile platforms for developers to implement AI and machine learning applications. Over the years, Nvidia has introduced several key products in the Jetson lineup, each advancing the capabilities and performance of embedded systems.  


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/jetsonevolution.webp" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Four steps to AI on Jetson, each on two legs.
</div>



#### Jetson TX2 (2017): Embedded AI

The release of the Jetson TX2 in 2017 marked a milestone in the development of embedded AI systems. Building on the success of its predecessors (TK1 and TX1), the TX2 introduced a more powerful and energy-efficient platform, making it suitable for real-time computer vision applications in edge devices.

The Jetson TX2 featured a Pascal GPU with 256 CUDA cores and a dual-core Denver 2 ARM CPU coupled with a quad-core ARM Cortex-A57. This architecture provided twice the performance of the TX1 while maintaining a similar power envelope. The TX2 found use cases in autonomous drones, robotics, and industrial automation, where real-time image processing and AI inference were essential. Its support for deep learning frameworks allowed developers to deploy AI models directly on the edge, reducing latency and improving time-sensitive performance.

#### Jetson Nano (2019): AI at the Edge

The Jetson Nano, introduced in 2019, offered a low-cost platform for embedded computer vision. Designed for hobbyists, researchers, and developers working on budget-constrained projects, the Jetson Nano provided easy access to AI and machine learning tools.

Despite its affordable price, the Jetson Nano featured a 128-core Maxwell GPU and a quad-core ARM Cortex-A57 CPU, making it powerful enough to handle real-time image classification, object detection, and segmentation tasks. It supported popular AI frameworks such as TensorFlow and PyTorch, enabling the deployment of deep learning models in various applications. The Jetson Nano became popular in robotics, smart cameras, and educational projects. Its affordability and ease of use made it a platform of choice for developers looking to experiment with AI and computer vision on a smaller scale, without sacrificing performance.

#### Jetson Xavier NX (2020): High-Performance AI in a Compact Form

In 2020, Nvidia introduced the Jetson Xavier NX, a compact yet powerful SBC designed to bridge the gap between the affordable Jetson Nano and the more robust Jetson AGX Xavier. The Xavier NX brought AI capabilities to edge devices that required a small footprint and low power consumption.

The Jetson Xavier NX featured a Volta GPU with 384 CUDA cores and 48 Tensor Cores, providing up to 21 TOPS (trillions of operations per second) of AI performance. This made it suitable for demanding computer vision tasks, such as multi-camera processing, video analytics, and autonomous robotics.

The Xavier NX offered a scalable solution for developers, allowing them to build AI-powered devices that could handle complex tasks in real-time. Its ability to process multiple high-resolution video streams simultaneously made it a good choice for applications like smart surveillance and advanced robotics.

#### Jetson Orin Nano (2023): Supercharged Entry-Level Applications

The Jetson Orin Nano, launched in 2023, represents the next generation of AI computing for entry-level embedded applications. Building on the success of the original Nano, the Orin Nano offers significantly enhanced performance and AI capabilities while maintaining an accessible price point.

The Jetson Orin Nano features the Ampere GPU architecture with up to 1024 CUDA cores, delivering up to 40 TOPS of AI performance. This is a substantial upgrade from the original Nano, enabling more complex AI models and real-time computer vision tasks to be executed on edge devices.

The Orin Nano is designed for applications where both cost and performance are necessary. It is well-suited for video analytics, and entry-level autonomous systems, helping developers to implement AI tasks without the need for higher-end hardware.

#### Jetson AGX Orin (2023): AI Supercomputing at the Edge

The Jetson AGX Orin, also released in 2023, stands at the top of Nvidia’s Jetson lineup, offering high performance for the demanding real-time embedded applications. Featuring the Ampere GPU architecture with up to 2048 CUDA cores and 64 Tensor Cores, the Jetson AGX Orin delivers up to 275 TOPS of AI performance. This processing capability enables the execution of the many complex AI models, including those used in autonomous vehicles, robotics, and industrial automation. Support for advanced AI frameworks and libraries makes Jetson AGX Orin an attractive platform for next-generation AI systems.

> Nvidia Jetson platforms have enabled a wide range of applications, from hobbyist projects to industrial automation and autonomous systems.

Nvidia Jetson single-board computers have shown how quickly real-time embedded computer vision and AI have advanced. Starting with the Jetson TX2, which offered a big jump in performance and efficiency, Nvidia made AI more accessible with the Jetson Nano. Now, with the powerful Jetson AGX Orin, they have brought supercomputing power to edge AI and embedded vision systems, constantly pushing the limits of what's possible.
