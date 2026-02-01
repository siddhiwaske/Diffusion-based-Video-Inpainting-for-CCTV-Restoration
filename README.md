# Diffusion-based-Video-Inpainting-for-CCTV-Restoration
Research-oriented project exploring diffusion-based video inpainting for restoring CCTV footage affected by real-world obstructions
## Overview
This project explores diffusion-based video inpainting techniques to restore CCTV footage affected by real-world obstructions such as leaves, dirt, and lens flare. The work focuses on designing a modular vision pipeline combining object detection, segmentation, and generative inpainting.

## Motivation
CCTV footage is often partially occluded due to environmental factors, which can limit its usability in surveillance and analysis tasks. This project was motivated by real-world scenarios where visual obstructions degrade video quality, and explores how generative models can assist in reconstructing missing visual information.

## Approach
The pipeline follows a multi-stage approach:
- Object detection to identify obstructed regions
- Segmentation-based mask generation
- Diffusion-based inpainting to reconstruct missing areas

Pre-trained models were explored to understand their behavior and limitations in real-world surveillance scenarios.

## Dataset
Due to the lack of publicly available datasets containing obstructed CCTV footage, a synthetic dataset was created by introducing controlled obstructions into video frames. This enabled experimentation under realistic conditions.

## Experiments & Observations
Experiments revealed challenges in handling multiple simultaneous obstructions and maintaining consistency across frames. While the inpainting results were visually promising, further refinement is required for robustness.

## Limitations & Future Work
This project is a research prototype and has several limitations:
- Lack of large-scale fine-tuning data
- Frame-level inconsistencies in complex scenes

Future work includes dataset expansion, fine-tuning diffusion models, and improving temporal coherence.

## Acknowledgements
This project builds upon the publicly available DiffuEraser repository:
[https://github.com/xxx/DiffuEraser](https://github.com/lixiaowen-xw/DiffuEraser)

The original implementation was used as a baseline for understanding diffusion-based video inpainting. All experiments and pipeline adaptations were conducted strictly for academic and research purposes.

## Disclaimer
This repository is intended for academic and learning purposes only. It does not represent a production-ready system.

