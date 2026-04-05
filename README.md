# Awesome Monocular Height Estimation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of papers, datasets, benchmarks, and code resources for **monocular height estimation (MHE)**, **single-view DSM / nDSM generation**, and **single-image building/object height estimation** from **overhead remote sensing imagery**.

This list focuses on **remote sensing** and related single-view height recovery from:
- aerial RGB imagery
- satellite optical imagery
- single SAR imagery
- shadow-/geometry-based single-image methods

It intentionally **excludes generic monocular depth estimation (MDE)** papers unless they are explicitly formulated or evaluated as **height estimation** in remote sensing.

## Contents
- [Awesome Monocular Height Estimation ](#awesome-monocular-height-estimation-)
  - [Contents](#contents)
  - [Surveys \& Overviews](#surveys--overviews)
  - [Classical Single-Image / Shadow-Based Methods](#classical-single-image--shadow-based-methods)
  - [CNN / Encoder-Decoder Methods](#cnn--encoder-decoder-methods)
  - [Multi-Task, Contrastive, and Label-Efficient Learning](#multi-task-contrastive-and-label-efficient-learning)
  - [Transformers \& Hybrid CNN-Transformer Methods](#transformers--hybrid-cnn-transformer-methods)
  - [Diffusion-Based Methods](#diffusion-based-methods)
  - [Single-SAR Height Estimation](#single-sar-height-estimation)
  - [Building-Centric / Object-Centric Height Estimation](#building-centric--object-centric-height-estimation)
  - [3D Reconstruction Closely Tied to Monocular Height Estimation](#3d-reconstruction-closely-tied-to-monocular-height-estimation)
  - [Benchmarks \& Datasets](#benchmarks--datasets)
  - [Code](#code)
  - [Evaluation Metrics](#evaluation-metrics)
  - [Related Topics](#related-topics)
  - [Contributing](#contributing)

---

## Surveys & Overviews

- **The Use of Deep Learning Methods for Object Height Estimation in High Resolution Satellite Images** (2023) — [Paper](https://www.mdpi.com/1424-8220/23/19/8162)
- **A Multi-Modal, Multi-Temporal, Multi-Resolution Benchmark Dataset for Building Height Estimation** (2026) — [Paper](https://www.nature.com/articles/s41597-025-06495-3)

---

## Classical Single-Image / Shadow-Based Methods

- **Height Determination of Extended Objects Using Shadows in SPOT Images** (1998)
- **Shadow Detection and Building-Height Estimation Using IKONOS Data** (2011) — [Paper](https://www.tandfonline.com/doi/full/10.1080/01431161.2010.517226)
- **3D Polygonal Building Model Estimation from Single Satellite Images** (2012) — [Paper](https://www2.ensc.sfu.ca/research/lrv/publications/journals/GRSS_DC.pdf)
- **Automatic Building Height Extraction by Volumetric Shadow Analysis of Monoscopic Imagery** (2013)
- **Shadow Analysis Technique for Extraction of Building Height Using High Resolution Satellite Single Image and Accuracy Assessment** (2014)
- **Satellite Images Analysis for Shadow Detection and Building Height Estimation** (2016)
- **Building Height Estimation Using Google Earth** (2016) — [Paper](https://www.sciencedirect.com/science/article/pii/S0378778816301025)
- **A Shadow-Overlapping Algorithm for Estimating Building Heights From VHR Satellite Images** (2018)
- **Multi-scene Building Height Estimation Method Based on Shadow in High Resolution Imagery** (2021)
- **Building Height Estimation from High Resolution Satellite Images** (2022)
- **Building Height Extraction From High-Resolution Single-View Remote Sensing Images Using Shadow and Side Information** (2024)
- **Building Height Estimation Using Shadow Length in Satellite Imagery** (2024) — [Paper](https://arxiv.org/abs/2411.09411)

---

## CNN / Encoder-Decoder Methods

- **IM2HEIGHT: Height Estimation from Single Monocular Imagery via Fully Residual Convolutional-Deconvolutional Network** (2018) — [Paper](https://arxiv.org/abs/1802.10249)
- **IMG2DSM: Height Simulation From Single Imagery Using Conditional Generative Adversarial Net** (2018)
- **Height Estimation from Single Aerial Images Using a Deep Convolutional Encoder-Decoder Network** (2019) — [Paper](https://www.sciencedirect.com/science/article/pii/S0924271619300139)
- **IM2ELEVATION: Building Height Estimation from Single-View Aerial Imagery** (2020) — [Paper](https://www.mdpi.com/2072-4292/12/17/2719)
- **Height Estimation from Single Aerial Images Using a Deep Ordinal Regression Network** (2020) — [Paper](https://arxiv.org/abs/2006.02801)
- **Generating Elevation Surface from a Single RGB Remotely Sensed Image Using Deep Learning** (2020) — [Paper](https://www.mdpi.com/2072-4292/12/12/2002)
- **StyHighNet: Semi-Supervised Learning Height Estimation from a Single Aerial Image via Unified Style Transferring** (2021)
- **IMG2nDSM: Height Estimation from Single Airborne RGB Images with Deep Learning** (2021) — [Paper](https://www.mdpi.com/2072-4292/13/12/2417)
- **Focusing on Shadows for Predicting Heightmaps from Single Remotely Sensed RGB Images with Deep Learning** (2021) — [Paper](https://arxiv.org/abs/2104.10874)
- **Height Estimation from Single Aerial Imagery with a Deep Boundary-Guided Network** (2021)
- **IMG2HEIGHT: Height Estimation from Single Remote Sensing Image Using a Deep Convolutional Encoder-Decoder Network** (2023) — [Paper](https://www.tandfonline.com/doi/full/10.1080/01431161.2023.2251185)
- **LUMNet: Land Use Knowledge Guided Multiscale Network for Height Estimation From Single Remote Sensing Images** (2024)
- **Estimation of the Height of Monocular Satellite Remote Sensing Images Based on Semantic Information Enhancement** (2025)
- **Single-Image Building Height Estimation Using Spatial Relation Enhancement** (2026)
- **RDAH-Net: Bridging Relative Depth and Absolute Height for Monocular Height Estimation in Remote Sensing** (2026) — [Paper](https://www.mdpi.com/2072-4292/18/7/1024)

---

## Multi-Task, Contrastive, and Label-Efficient Learning

- **Multitask Learning of Height and Semantics From Aerial Images** (2019)
- **Multi-Task Learning of Relative Height Estimation and Semantic Segmentation from Single Airborne RGB Images** (2022) — [Paper](https://www.mdpi.com/2072-4292/14/14/3450)
- **Knowledge Transfer for Label-Efficient Monocular Height Estimation** (2022)
- **Joint Learning of Semantic Segmentation and Height Estimation for Remote Sensing Image Leveraging Contrastive Learning** (2023)
- **Height Estimation from Single Aerial Imagery Using Contrastive Learning Based Multi-Scale Refinement Network** (2023) — [Paper](https://www.tandfonline.com/doi/full/10.1080/17538947.2023.2225881)
- **Adaptive Bins for Monocular Height Estimation from Single Remote Sensing Images** (2023)
- **Long-tailed Regression with Ensembles for Monocular Height Estimation from Single Remote Sensing Images** (2023)
- **Enhancing Monocular Height Estimation via Sparse LiDAR-Guided Correction** (2025) — [Paper](https://arxiv.org/abs/2505.06905)

---

## Transformers & Hybrid CNN-Transformer Methods

- **THE Benchmark: Transferable Representation Learning for Monocular Height Estimation** (2021) — [Paper](https://arxiv.org/abs/2112.14985)
- **HTC-DC Net: Monocular Height Estimation From Single Remote Sensing Images** (2023) — [Paper](https://arxiv.org/abs/2309.16486)
- **HeightFormer: A Multilevel Interaction and Image-Adaptive Classification-Regression Network for Monocular Height Estimation with Aerial Images** (2024) — [Paper](https://arxiv.org/abs/2310.07995)
- **Height Estimation from Monocular Aerial Images Using Convolutional Multi-Scale and Transformer Coupling Network (CMT)** (2025) — [Paper](https://www.sciencedirect.com/science/article/pii/S0924271625002710)
- **Fusing Convolution and Vision Transformer Encoders for Object Height Estimation from Monocular Satellite and Aerial Images** (2025) — [Paper](https://openaccess.thecvf.com/content/ICCV2025W/3D-VAST/papers/Gultekin_Fusing_Convolution_and_Vision_Transformer_Encoders_for_Object_Height_Estimation_ICCVW_2025_paper.pdf)

---

## Diffusion-Based Methods

- **Single-View Height Estimation with Conditional Diffusion Probabilistic Models** (2023) — [Paper](https://arxiv.org/abs/2304.13214)

---

## Single-SAR Height Estimation

- **Deep-Learning-Based Single-Image Height Reconstruction from Very-High-Resolution SAR Intensity Data** (2022) — [Paper](https://www.sciencedirect.com/science/article/pii/S0924271621003105)
- **From Relative to Absolute Heights in SAR-based Single-Image Height Prediction** (2023)
- **A Geometry-Aware Consistent Constraint for Height Estimation from a Single SAR Imagery in Mountain Areas** (2023)
- **The SAR2Height Framework for Urban Height Map Reconstruction from Single SAR Intensity Images** (2024) — [Paper](https://www.sciencedirect.com/science/article/pii/S0924271624000959)
- **An Object-Based Deep Learning Approach for Building Height Estimation from Single SAR Images** (2025) — [Paper](https://arxiv.org/abs/2507.08096)

---

## Building-Centric / Object-Centric Height Estimation

- **3DCentripetalNet: Building Height Retrieval from Monocular Remote Sensing Imagery** (2023) — [Paper](https://www.sciencedirect.com/science/article/pii/S1569843223001334)
- **HeightNet: Monocular Object Height Estimation** (2023) — [Paper](https://www.mdpi.com/2079-9292/12/2/350)
- **A Robust Method for Roof Extraction and Height Estimation** (2023)
- **Monocular Building Height Estimation from PhiSat-2 Imagery** (2026) — [Paper](https://arxiv.org/abs/2603.29245)

---

## 3D Reconstruction Closely Tied to Monocular Height Estimation

> These papers are not pure “height-map only” prediction papers, but they contain single-view remote sensing **elevation estimation modules** directly relevant to MHE.

- **Elevation Estimation-Driven Building 3-D Reconstruction from Single-View Remote Sensing Imagery** (2023)
- **3D Building Reconstruction from Monocular Remote Sensing Images with Multi-level Roof Contours Prediction** (2024) — [Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_3D_Building_Reconstruction_from_Monocular_Remote_Sensing_Images_with_Multi-level_CVPR_2024_paper.pdf)
- **3D Building Reconstruction from Monocular Remote Sensing Imagery via Diffusion Models and Geometric Priors** (2026)

---

## Benchmarks & Datasets

- **THE Benchmark** (2021) — cross-dataset transfer benchmark for MHE — [Project](https://thebenchmarkh.github.io/)
- **MAMHESet: A Multiangle Monocular Height Estimation Dataset From Luojia3-01 Video Satellite** (2025)
- **M4Heights** (2026) — large-scale benchmark dataset for building height estimation — [Paper](https://www.nature.com/articles/s41597-025-06495-3)
- **ISPRS Vaihingen** — widely used for single-view DSM / nDSM estimation
- **ISPRS Potsdam** — widely used for aerial-image height prediction
- **DFC2019 / GRSS Data Fusion Contest** — common MHE evaluation benchmark
- **GBH** — used in HTC-DC Net and later MHE papers
- **PhiSat-2 building height benchmark** (2026)

---

## Code

- **HTC-DC Net** — [GitHub](https://github.com/zhu-xlab/HTC-DC-Net)
- **ImageToDEM / Generating Elevation Surface from a Single RGB Remotely Sensed Image Using Deep Learning** — [GitHub](https://github.com/Panagiotou/ImageToDEM)
- **THE Benchmark** — [Project](https://thebenchmarkh.github.io/)
- **M4Heights baselines / benchmark context** — [Dataset paper](https://www.nature.com/articles/s41597-025-06495-3)

---

## Evaluation Metrics

Common metrics used in MHE / single-view DSM estimation:

- **MAE** — Mean Absolute Error
- **RMSE** — Root Mean Square Error
- **ME** — Mean Error / Bias
- **Log RMSE**
- **\(R^2\)** / correlation
- **δ-accuracy** style thresholds (less common than in generic MDE, but still used in some work)
- **Per-building MAE / RMSE**
- **Boundary quality / sharpness**
- **Generalization across cities / sensors / resolutions**

---

## Related Topics

- Monocular depth estimation for remote sensing
- Single-view DSM / nDSM generation
- Single-view 3D building reconstruction
- Building footprint extraction
- Shadow detection in overhead imagery
- Single-image SAR interpretation
- Geospatial foundation models

---

## Contributing

Contributions are welcome.

Please ensure that additions:
- are **explicitly about height estimation**, single-view DSM/nDSM generation, or building/object height recovery from remote sensing imagery;
- are **not generic monocular depth papers** unless height estimation is a central formulation;
- include a **paper link** and, if available, **code/project link**;
- are placed in the most appropriate section.

---

## License

[CC0](https://creativecommons.org/publicdomain/zero/1.0/)
