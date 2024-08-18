---
layout: page
title: WildSight
description: Precision wildlife detection with deep learning
img: assets/img/wildsight.webp
importance: 1
category: work
related_publications: true
---

### Motivation
Collisions between vehicles and animals present a significant issue in numerous countries, making it crucial to predict accidents and associated costs at regional and national levels for effective accident prevention {% cite GREN2019112 %}.

Furthermore, a recent bear encounter at a clinic in Niigata Prefecture reflects a worrying trend of bears moving closer to human settlements in Japan. Due to a shortage of acorns, their primary food, and the spread of untamed vegetation, bears are increasingly foraging near human areas. A new term, "shin-sedai kuma" or "new-generation bears," describes those born near human communities who are less afraid of people. This shift in bear behavior highlights the need for greater caution and a reassessment of human-bear interactions.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/bearsdetectbb.png" title="WildSight Algotechniq" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Detecting bears and cars by Algotechniq's WildSight.
</div>

### Objective
   The goal of the WildSight project is to improve the accuracy and robustness of wild animal detection in complex field scenarios by using the [YOLOv8](https://resources.wolframcloud.com/NeuralNetRepository/resources/YOLO-V8-Detect-Trained-on-MS-COCO-Data/) algorithm. The focus is on localizing and recognizing wild animals in different challenging environments, including scenes with multiple targets, small targets, or obstructed targets.

### Prior Work
   Previously, wild animal detection relied heavily on manual observation and feature-based algorithms, such as the HOG (Histogram of Oriented Gradients), and DPM (Deformable Parts Model) algorithms. These methods involved manually designed features and detectors, which were limited by their inability to achieve high accuracy and robustness in complex scenes. More recently, deep learning-based methods, particularly transfer learning techniques, have been used but lacked the real-time performance needed for field applications {% cite 10.1007/978-3-031-62281-6_30 %}.

### Benefits
- Municipalities and safety authorities can deploy this technology to monitor and manage the presence of wild animals in urban or suburban areas. Early detection of animals near roads, residential areas, or public spaces can help prevent accidents, such as vehicle collisions with large animals, thereby improving public safety.

- Other  beneficiaries include biologists and researchers involved in wildlife monitoring and conservation. The approach can also be valuable to photographers, drone operators, and others involved in outdoor exploration and wildlife studies who require accurate and efficient animal detection in various environmental conditions.

### Enabling Technologies
   The key enabling technologies of the new approach include:
   - YOLOv8 is a new real-time object detection algorithm that builds upon earlier YOLO versions, offering enhanced accuracy and speed, for images and videos.
   - [Data Augmentation Techniques](https://en.wikipedia.org/wiki/Data_augmentation) to enhance the training dataset and improve model robustness.

### Performance Criteria
   The success of the new approach can be quantified through metrics such as precision, recall, mean Average Precision (mAP), and loss function trends during training. Additionally, the model's ability to perform well in complex scenarios, such as detecting multiple, occluded, or small targets, serves as further evidence of its success.