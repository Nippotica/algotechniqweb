---
layout: page
title: AutoClaim AI
description: Precision damage detection for smarter insurance
img: assets/img/autoclaim.webp
importance: 3
category: work
related_publications: true
---



### Objective
This project focuses on developing a deep learning-based approach to automatically detect, locate, and categorize vehicle damage. The innovation lies in the ability to assess damage severity and visually highlight it on the vehicle's image, offering a fully automated damage assessment tool.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/autoclaim.webp" title="Autoclaim Algotechniq" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A picture is all you need to file car insurance claims.
</div>

### Prior Work
Previously, vehicle damage detection was achieved using various computer vision and deep learning techniques, such as convolutional neural networks (CNNs) and transfer learning {% cite VANRUITENBEEK2022100332 %}. However, these methods were primarily focused on identifying damage without providing detailed severity classification or localization of the damage. The earlier methods were also limited by the inability to assess damage severity or precisely locate it {% cite Mallios10194904 %}.

### Benefits
Insurance companies are the primary beneficiaries of this new approach. The enhanced accuracy and automation in detecting and classifying vehicle damage will help reduce claims leakage, speed up the claims processing, and reduce costs associated with manual damage assessment. Additionally, customers may benefit from faster and more accurate claims processing.

### Enabling Technologies
The key enabling technologies include:

- Mask R-CNN: An enhanced version of Faster R-CNN for object detection and instance segmentation, which includes a new RoIAlign layer for better accuracy.

- Transfer Learning: Utilizing pre-trained models like Inception V3 to extract features and reduce training time.

- Instance Segmentation: A technique to identify and classify different parts of an image, which is crucial for determining the severity of vehicle damage.

### Measuring Success
The success of our approach is quantified using performance metrics such as Precision, Recall, F1 Score, Accuracy, and the Loss Function. These metrics are applied to assess the performance of the deep learning models used in terms of their ability to detect, localize, and classify vehicle damage. The model's effectiveness is further validated using confusion matrices and empirical results showing that the proposed method outperforms previous approaches in all categories of detection, localization, and severity classification.