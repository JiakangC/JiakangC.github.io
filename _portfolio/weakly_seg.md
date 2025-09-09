---
title: "Ensembled Weakly-Supervised Segmentation"
collection: portfolio
permalink: /portfolio/ensembled-segmentation
date: 2024-06-01
excerpt: "An MSc Machine Learning project developing an ensembled model for weakly-supervised image segmentation. <br/><img src='/images/WSSS_Flow.png'>"
tags:
  - Machine Learning
  - Computer Vision
  - Weakly-Supervised Learning
---

This project explores **ensembled weakly-supervised segmentation** techniques for computer vision tasks.  
The goal was to leverage multiple models to improve segmentation accuracy under limited supervision, combining ideas from deep learning, ensembling, and semi-supervised learning.  

Weakly supervised semantic segmentation (WSSS) reduces the cost of pixel-level annotation by training models with only image-level labels. In this work, we first establish a unified benchmark evaluating three CAM-based localization methods—CAM, Erased CAM (ECS-CAM), and Contrastive CAM (CCAM)—under identical training and augmentation protocols. Building on their complementary strengths, we propose an ensemble framework that fuses multi-method activation maps and applies a lightweight CRF-based refinement to produce high-quality pseudo-pixel labels. To further improve mask completeness and background suppression, we introduce two novel training strategies: (1) augmenting with background-only images by adding a “bg” class, and (2) a pet-specific contrastive fine-tuning stage that treats each breed as a separate category within CCAM. Finally, we use these pseudo-labels to train a U-Net segmentation network and compare its performance against a fully supervised U-Net baseline. Our best weakly supervised model achieves 61.6 \%(finetune) and 76 \%(pretrain) IoU comparing to the 68.25 \% on fully supervised baseline model. 

👉 [View Repository on GitHub](https://github.com/JiakangC/Ensembled-Weakly-Supervised-Segmentation)

📄  [Read Full Dissertation (PDF)](/files/ADL_WSSS.pdf)