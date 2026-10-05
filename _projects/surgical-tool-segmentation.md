---
title: Surgical Tool Instance Segmentation
summary: A YOLO26 + SAM2 pipeline that segments surgical instruments in laparoscopic gallbladder surgery video, outperforming the Mask R-CNN and Mask2Former baselines from the original study.
tags: [Computer Vision, YOLO26, SAM2, PyTorch]
github: https://github.com/DataScientistRN/Surgical-Tool-Instance-Segmentation-Spring-2026
icon: scalpel
color: peach
order: 1
---

*CSCI E-25 Computer Vision · Spring 2026*

As minimally invasive and robotic surgery becomes more common, precise segmentation of surgical tools is a building block for computer-assisted and eventually autonomous surgical systems.

This project fine-tunes YOLO26 on the CholecInstanceSeg dataset (41,933 annotated frames from 85 laparoscopic cholecystectomies, seven instrument classes) and pairs it with SAM2 for high-quality masks. A custom augmentation pipeline targets class imbalance, with the biggest gains on the rarest instruments.

The fine-tuned baseline already beat both models from the original study on mAP(50-95), and the augmented model outperformed all three, reaching 74.0 overall against 61.5 for Mask2Former.

![Per-class mAP(50-95) for Mask R-CNN, Mask2Former and the two YOLO26 models]({{ '/assets/img/surgical-tools-results.png' | relative_url }})
