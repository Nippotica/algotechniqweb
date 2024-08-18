---
layout: page
title: ConcreteVision
description: Real-time concrete pouring monitor
img: assets/img/concretevision.webp
importance: 3
category: work
related_publications: true
---

### Motivation
The Concrete Layer Coverage Interval (CLCI) is the critical time between when concrete is poured and when it needs to be covered to maintain proper moisture and temperature for curing. 

Proper coverage prevents issues like cracking and weakening due to exposure to environmental factors. Overtime alerts for CLCI are essential because they notify construction teams if the concrete isn't covered in time, helping to preserve its structural integrity and durability. This real-time alert system ensures that the concrete cures correctly, reducing the risk of defects and ensuring the safety and quality of the structure.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/concretetruck.jpg" title="concrete truck" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/constructionsite.jpg" title="construction site" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### Objective
   The project introduces a new approach for monitoring the progress of concrete pouring in construction using deep object detection and semantic segmentation models. The specific novelty lies in achieving high  accuracy for overtime alerting of concrete layer coverage intervals, which improves the precision and timeliness of construction monitoring.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/concretevision.webp" title="ConcreteVision Algotechniq" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Algotechniq's AI Vision Transformer Monitoring Concrete Flow.
</div>

### Prior Work
   The monitoring of concrete pouring progress and quality control was primarily done manually. This manual approach often led to issues such as insufficient timeliness, misreporting, and omission of critical data, which could negatively impact the overall construction quality.

### Benefits
   Algotechniq’s technology will benefit construction management teams by providing more accurate, real-time data on construction progress. This improvement supports better quality control, progress tracking, and overall productivity analysis in construction projects, particularly in large-scale infrastructure projects.

### Enabling Technologies
   The key enabling technologies include deep learning, computer vision techniques such as semantic segmentation and object detection, and advanced data processing methods like data augmentation and model training on specialized datasets. The use of Vision Transformers (ViTs) {% cite Arnab9710415 %}, pre-trained on large datasets  and fine-tuned for specific construction scenarios, is central to this approach.

### Quantifying Performance
   The success of the new approach can be quantified by the accuracy and timeliness of the overtime warnings for concrete layer coverage intervals. Specifically, the approach is evaluated by comparing the model's predictions with manually annotated real-world data, ensuring that the model can accurately detect the construction progress and provide timely warnings to prevent delays. 

