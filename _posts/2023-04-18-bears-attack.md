---
layout: post
title: Claws of Concern
date: 2023-04-18
description: Bears attacking Japan
tags: technote
categories: Algoblog
---

> Japan has recently faced a troubling surge in bear attacks. 

These incidents, which have shaken the nation, reflect a growing tension between humans and wildlife, exacerbated by environmental and societal factors.

The frequency of bear encounters has notably increased in rural and even suburban areas. As of 2024, Japan has reported over 50 bear attacks, with several resulting in fatalities. The prefectures of Akita, Iwate, and Yamagata have been particularly affected, where residents and authorities are on high alert.


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/hfLTt-ZQNoc?si=cMPkry4OSdEH5f-n" class="rounded z-depth-1" controls=true width=400 height=225 %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/pLN11JicH5U?si=Se0VbykCCUinlZ1H" class="rounded z-depth-1" controls=true width=400 height=225 %}
    </div>
</div>


Several factors contribute to this rise in bear activity. Climate change is altering the natural habitats and food sources of bears, pushing them closer to human settlements in search of sustenance. Additionally, Japan’s aging rural population has led to abandoned farmlands, creating an environment where bears can roam more freely without human deterrence. The decrease in hunting and trapping, partly due to stricter regulations and a declining interest in these activities among younger generations, has also led to a population increase in certain bear species.

The government has responded with heightened measures, including increased patrolling of bear-prone areas, public awareness campaigns, and in some cases, culling to control the population. However, these measures have sparked debate, balancing between wildlife conservation and human safety.

Experts suggest that a long-term solution requires addressing the root causes, such as habitat preservation and better waste management, to prevent bears from entering human spaces. The situation underscores the need for a sustainable coexistence strategy between humans and wildlife in Japan, ensuring safety while preserving the country’s natural heritage.

### Algotechniq's Approach

At Algotechniq, we're developing deep learning algorithms for locating and recognizing wild animals in different challenging environments, including scenes with multiple targets, small targets, or obstructed targets.

Our algorithm, incorporated into our WildSight product, runs on Jetson Nano where it takes in scene video at 30 fps and outputs a bounding box around the animal. 


<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="/assets/video/beardetect3.mp4" class="img-fluid rounded z-depth-1" controls=true  type="video/mp4" %}
    </div>
</div>
<div class="caption">
    Locating a running bear by Algotechniq's WildSight. 
</div>

The above video is extracted from [Nippon TV News Japan](https://www.youtube.com/watch?v=pLN11JicH5U).

