# EgoEv-HandPose
Official PyTorch implementation of the paper "EgoEV-HandPose: Egocentric 3D Hand Pose Estimation and Gesture Recognition Based on Binocular Event Cameras". Code, pre-trained models, dataset links, and experiment results are to be uploaded.

<img width="11482" height="2973" alt="fig1" src="https://github.com/user-attachments/assets/34336cc6-2375-4bff-80cb-ac704ce11ab2" />
*Fig. 1: Overview of the proposed EgoEV-HandPose framework and the established EgoEVHands dataset. The framework addresses the current challenges of RGB-based or monocular systems, such as lighting sensitivity and depth ambiguity, by introducing EgoEVHands, to the best of our knowledge, the first large-scale, real-world stereo event-based dataset for egocentric hand perception, characterized by its HDR properties, 3D geometric constraints, and bimanual interactions.*

## Project Overview

Egocentric 3D hand pose estimation and gesture recognition are essential for immersive augmented/virtual reality, human-computer interaction, and robotics. However, conventional frame-based cameras suffer from motion blur and limited dynamic range, while existing event-based methods are hindered by ego-motion interference, monocular depth ambiguity, and the lack of large-scale real-world stereo datasets.

To overcome these limitations, we propose **EgoEV-HandPose**, an end-to-end framework for joint 3D bimanual pose estimation and gesture recognition from stereo event streams. Central to our approach is **KeypointBEV**, a flexible stereo fusion module that lifts features into a canonical bird's-eye-view space and employs an iterative reprojection-guided refinement loop to progressively resolve depth uncertainty and enforce kinematic consistency.

In addition, we introduce **EgoEVHands**, the first large-scale real-world stereo event-camera dataset for egocentric hand perception, containing 5,419 annotated sequences with dense 3D/2D keypoints across 38 gesture classes under varying illumination.

Extensive experiments demonstrate that EgoEV-HandPose achieves state-of-the-art performance with:
- **30.54 mm MPJPE** (Mean Per-Joint Position Error) for 3D hand pose estimation
- **86.87% Top-1 accuracy** for gesture recognition
- Significant robustness in low-light and bimanual occlusion scenarios

## Updates
- [x] Paper published
- [ ] Source code release
- [ ] Pre-trained models release
- [ ] EgoEVHands dataset release

Code, pre-trained models, dataset links, and experiment results will be uploaded soon.

## Citation
If you find this work useful, please cite our paper:

@article{wang2026egoev,

title={EgoEV-HandPose: Egocentric 3D Hand Pose Estimation and Gesture Recognition with Stereo Event Cameras},

author={Wang, Luming and Shi, Hao and Zhai, Jiajun and Yang, Kailun and Wang, Kaiwei},

journal={ https://arxiv.org/pdf/2605.12297 },

year={2026}}
