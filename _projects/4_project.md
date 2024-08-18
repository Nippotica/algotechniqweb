---
layout: page
title: SmartScan
description: Detecting surface defects with deep learning
img: assets/img/smartscan.webp
importance: 2
category: work
related_publications: true
---

### Objective
   The goal of this project is to create a large-scale metallic surface defect detection system that is more robust and accurate in real-world industrial environments. This is achieved by using datasets that include defect types collected from real industry situations, and by proposing an end-to-end defect detection network that combines inferences from several deep learning and data augmentation techniques.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/smartscan.webp" title="SmartScan Algotechniq" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Illustrating typical defects on a metallic surface.
</div>

### Prior Work
   Previously, defect detection for metallic surfaces relied on traditional image processing algorithms that utilized hand-crafted features, such as local binary patterns (LBP) and histogram of oriented gradients {% cite jimaging9100193 %}. These methods, while effective in controlled environments, performed poorly in varying industrial applications due to their sensitivity to environmental factors like lighting and background clutter. Deep learning methods were also used {% cite arikan2019surface %}., but they were often limited by the scale and diversity of the datasets available for training.

### Benefits
   Industries that require high-quality control for metallic products will benefit from the new approach, particularly those involved in manufacturing processes where surface defects can significantly impact product quality. The improved robustness and accuracy of the defect detection system will help in reducing manual inspection costs and improving the overall efficiency of the production line.

### Enabling Technologies
   The key enabling technologies of the new approach include:
- Faster R-CNN: High accuracy using a two-stage process with region proposals, but slower than the older Single Shot MultiBox Detector (SSD).
- YOLO: Fast and suitable for real-time detection, but less accurate for small objects and dense scenes.
- RetinaNet: Balances speed and accuracy, with improved detection of small objects using focal loss.
- EfficientDet: Optimized for both speed and accuracy, scalable for various resource constraints. 
- Data augmentation methods, which are used to expand the training dataset and improve the model's robustness to various defect shapes and sizes.

Each offers different trade-offs between speed, accuracy, and complexity.

### Quantifying Results
   The success of our approach can be quantified using performance metrics such as Recall, Average Precision (AP), and mean Average Precision (mAP) across different defect categories. The approach's effectiveness is demonstrated by its superior performance on these metrics compared to previous methods, as well as its ability to detect defects in real-time with a fast processing speed per image. 




