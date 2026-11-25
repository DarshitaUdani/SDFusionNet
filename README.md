# SDFusionNet

### A Novel Multimodal Fusion Framework for Robust Person Identification

## Overview

**SDFusionNet** is a computer vision research project focused on human identification through skeleton-based feature representation and dynamic feature fusion.

The project explores the integration of multiple complementary feature representations to improve identification performance under varying viewpoints. It combines motion-based, skeletal, and statistical information through a unified architecture designed to learn discriminative identity representations.

The proposed framework incorporates canonical skeleton normalization, dynamic feature extraction, and adaptive gated fusion to generate robust feature embeddings for identity classification.

## Architecture

The SDFusionNet framework consists of the following major components:

1. **Canonical Skeleton Normalization**
   - Normalizes skeletal representations into a canonical coordinate system.
   - Reduces variations caused by differences in body orientation and viewpoint.

2. **DynoFusion Module**
   - Integrates multiple feature extraction branches.
   - Incorporates MotionNet-X, TransMotion, SkeleGraph encoders, and a statistical feature branch.
   - Captures complementary motion and skeletal characteristics.

3. **Adaptive Gated Fusion**
   - Dynamically combines features from different branches.
   - Learns adaptive weights to balance the contribution of individual feature representations.

4. **Identity Embedding and Classification**
   - Generates a unified identity representation.
   - Uses the learned embeddings for human identity classification.

## Repository Structure

```text
SDFusionNet/
│
├── SDFusionNet.ipynb
│
├── attentionfusion.ipynb
│
├── basicconcatenation.ipynb
│
└── README.md
```

### Notebook Descriptions

| Notebook | Description |
|---|---|
| `SDFusionNet.ipynb` | Main implementation and experimentation of the SDFusionNet framework. |
| `attentionfusion.ipynb` | Exploration of attention-based feature fusion. |
| `basicconcatenation.ipynb` | Implementation of basic feature concatenation as a fusion approach. |

## Feature Fusion Approaches

The project explores different strategies for combining feature representations:

- **Basic Concatenation:** Combines extracted features into a unified representation through concatenation.
- **Attention-Based Fusion:** Explores attention mechanisms to learn the relative importance of different feature representations.
- **Adaptive Gated Fusion:** Integrates complementary features using learnable gating mechanisms within the proposed framework.

## Evaluation

The project considers multiple evaluation perspectives to investigate the robustness of the learned identity representations:

- Viewpoint-specific evaluation.
- Viewpoint-agnostic evaluation.
- Base model versus Test-Time Adaptation (TTA) comparison.
- Confusion matrix analysis.
- Cumulative Matching Characteristics (CMC) curves.
- Radar-based performance comparisons.
- Dataset viewpoint distribution analysis.

## Technologies

- Python
- Jupyter Notebook
- Deep Learning
- Computer Vision
- Neural Networks
- Feature Extraction and Representation Learning
- Attention Mechanisms
- Feature Fusion

## Research Objective

The primary objective of SDFusionNet is to investigate how complementary skeletal and motion-based representations can be effectively integrated to achieve robust human identification across different viewpoints.

By combining multiple feature extraction strategies with adaptive fusion, the framework aims to learn more discriminative and viewpoint-robust identity representations.

## Project Status

Research and experimentation are ongoing. The repository contains the main framework implementation and supporting feature fusion experiments.
