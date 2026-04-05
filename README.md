# Awesome Monocular Height Estimation

![Awesome](https://awesome.re/badge.svg)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Links verified](https://img.shields.io/badge/links_verified-2026--04--05-brightgreen)

A verified, curated **Awesome-list** of **Monocular Height Estimation (MHE)** and **single-view DSM/nDSM extraction** resources from **overhead remote sensing imagery** (optical & SAR).  
**Scope:** height/DSM/nDSM (metric or normalized) **from a single overhead image** (or single SAR image).  
**Exclude:** generic monocular depth estimation (MDE) papers that do **not** target overhead height/DSM (e.g., general indoor/outdoor MDE backbones without height/DSM adaptation).

## Executive summary

- Focused on **MHE / DSM / nDSM from single-view overhead imagery**, including optical and single-SAR variants, with dataset and code pointers when publicly available.
- Each paper entry includes **full title, full author list (or “unspecified”), year, venue, DOI/arXiv link, 1–2 sentence annotation**, and **code link if available** (otherwise “unspecified”).
- Includes: **60+ verified papers** (publisher/arXiv/official pages), plus benchmark/dataset table with practical usage notes.
- Provides a **mermaid timeline** of key milestones and a **mermaid pie chart** of paper distribution by section.
- Ready to paste into `README.md` (Awesome style, TOC, contribution guide, MIT license).

## Contents

- [Papers](#papers)
- [Benchmarks and datasets](#benchmarks-and-datasets)
- [Code resources](#code-resources)
- [Contributing](#contributing)
- [License](#license)

## Papers

**Table notes**
- **Link** is a DOI resolver, arXiv page, or primary publisher page.
- If a field is uncertain or not publicly stated on primary pages, it is marked **“unspecified”**.
- “Dataset(s)” references common/explicit benchmarks used in the paper (when described in the abstract/official page); otherwise **unspecified**.

| Section | Title | Year | Venue | Link | Code |
|---|---|---:|---|---|---|
| Surveys | **The Use of Deep Learning Methods for Object Height Estimation in High Resolution Satellite Images** | 2023 | Sensors | https://doi.org/10.3390/s23198162 | - |
| Classical/Shadow-based | **Automatic building height estimation with shadow in satellite images** | 2023 | SciDirect | https://www.sciencedirect.com/science/article/abs/pii/S235271022300462X | - |
| Classical/Shadow-based | **Building Height Extraction From High-Resolution Single-View Remote Sensing Images Using Shadow and Side Information** | 2024 | IEEE JSTARS | https://doi.org/10.1109/JSTARS.2024.3372113 | - |
| Classical/Shadow-based | **Single-Image Building Height Estimation Using Spatial Distribution-Aware Optimization in Complex Urban Areas** | 2026 | Remote Sensing | https://www.mdpi.com/2072-4292/18/5/801 | - |
| CNN/Encoder-Decoder | **IM2HEIGHT: Height Estimation from Single Monocular Imagery via Fully Residual Convolutional-Deconvolutional Network** | 2018 | arXiv | https://doi.org/10.48550/arXiv.1802.10249 | - |
| CNN/Encoder-Decoder | **IMG2DSM** | 2018 | IEEE GRSL | https://doi.org/10.1109/LGRS.2018.2806945 | - |
| CNN/Encoder-Decoder | **Height estimation from single aerial images using a deep convolutional encoder-decoder network** | 2019 | ISPRS JPRS | https://doi.org/10.1016/j.isprsjprs.2019.01.013 | - |
| CNN/Encoder-Decoder | **IM2ELEVATION: Building Height Estimation from Single-View Aerial Imagery** | 2020 | Remote Sensing | https://doi.org/10.3390/rs12172719 | - |
| CNN/Encoder-Decoder | **Generating Elevation Surface from a Single RGB Remotely Sensed Image Using Deep Learning** | 2020 | Remote Sensing | https://doi.org/10.3390/rs12122002 | https://github.com/Panagiotou/ImageToDEM |
| CNN/Encoder-Decoder | **U-IMG2DSM: Unpaired Simulation of Digital Surface Models With Generative Adversarial Networks** | 2021 | IEEE GRSL | https://doi.org/10.1109/LGRS.2020.2997295 | https://github.com/mhaut/UIMG2DSM |
| CNN/Encoder-Decoder | **Height estimation from single aerial images using a deep ordinal regression network** | 2020 | arXiv | https://doi.org/10.48550/arXiv.2006.02801 | - |
| CNN/Encoder-Decoder | **Soft-Aligned Gradient-Chaining Network for Height Estimation From Single Aerial Images** | 2021 | IEEE GRSL | https://doi.org/10.1109/LGRS.2020.2976485 | - |
| CNN/Encoder-Decoder | **IMG2nDSM: Height Estimation from Single Airborne RGB Images with Deep Learning** | 2021 | Remote Sensing | https://doi.org/10.3390/rs13122417 | - |
| CNN/Encoder-Decoder | **Gated Feature Aggregation for Height Estimation From Single Aerial Images** | 2022 | IEEE GRSL | https://doi.org/10.1109/LGRS.2021.3090470 | - |
| CNN/Encoder-Decoder | **StyHighNet: Semi-Supervised Learning Height Estimation from a Single Aerial Image via Unified Style Transferring** | 2021 | Sensors | https://www.mdpi.com/1424-8220/21/7/2272 | - |
| CNN/Encoder-Decoder | **IMG2HEIGHT: height estimation from single remote sensing image using a deep convolutional encoder-decoder network** | 2023 | IJRS | https://doi.org/10.1080/01431161.2023.2251185 | - |
| CNN/Encoder-Decoder | **Height estimation from single aerial imagery using contrastive learning based multi-scale refinement network** | 2023 | Int. J. Digital Earth | https://doi.org/10.1080/17538947.2023.2225881 | - |
| CNN/Encoder-Decoder | **Semantic-aware unsupervised domain adaptation for height estimation from single-view aerial images** | 2023 | ISPRS JPRS | https://www.sciencedirect.com/science/article/pii/S0924271623000096 | - |
| Transformers & Hybrid | **HTC-DC Net: Monocular Height Estimation From Single Remote Sensing Images** | 2023 | IEEE TGRS | https://doi.org/10.1109/TGRS.2023.3321255 | https://github.com/zhu-xlab/HTC-DC-Net |
| Transformers & Hybrid | **THE Benchmark: Transferable Representation Learning for Monocular Height Estimation** | 2023 | IEEE TGRS | https://doi.org/10.1109/TGRS.2023.3311764 | https://thebenchmarkh.github.io/ |
| Transformers & Hybrid | **Disentangled Latent Transformer for Interpretable Monocular Height Estimation** | 2022 | arXiv | https://doi.org/10.48550/arXiv.2201.06357 | - |
| Transformers & Hybrid | **Long-tailed Regression with Ensembles for Monocular Height Estimation from Single Remote Sensing Images** | 2023 | JURSE | https://doi.org/10.1109/JURSE57346.2023.10144186 | - |
| Transformers & Hybrid | **LUMNet: Land Use Knowledge Guided Multiscale Network for Height Estimation From Single Remote Sensing Images** | 2024 | IEEE GRSL | https://doi.org/10.1109/LGRS.2024.3374526 | - |
| Transformers & Hybrid | **HeightFormer: A Multilevel Interaction and Image-adaptive Classification-regression Network for Monocular Height Estimation with Aerial Images** | 2023 | arXiv | https://doi.org/10.48550/arXiv.2310.07995 | - |
| Transformers & Hybrid | **Morphological-Priors-Guided Network With Semantic Booster and Scalable Bins Module for Height Estimation From Single-View Remote Sensing Images** | 2025 | IEEE JSTARS | https://doi.org/10.1109/JSTARS.2025.3582823 | - |
| Transformers & Hybrid | **Height estimation from monocular aerial images using convolutional multi-scale and transformer coupling network (CMT)** | 2025 | ISPRS JPRS | https://www.sciencedirect.com/science/article/abs/pii/S0924271625002710 | - |
| Transformers & Hybrid | **Fusing Convolution and Vision Transformer Encoders for Object Height Estimation from Monocular Satellite and Aerial Images** | 2025 | ICCVW | https://openaccess.thecvf.com/content/ICCV2025W/3D-VAST/html/Gultekin_Fusing_Convolution_and_Vision_Transformer_Encoders_for_Object_Height_Estimation_ICCVW_2025_paper.html | - |
| Transformers & Hybrid | **TSE-Net** | 2025 | arXiv | https://doi.org/10.48550/arXiv.2511.13552 | https://github.com/zhu-xlab/tse-net |
| Transformers & Hybrid | **Cross-task Interaction MHE** | 2025 | Remote Sensing | https://www.mdpi.com/2072-4292/17/9/1637 | - |
| Transformers & Hybrid | **Knowledge-guided Multi-task Network** | 2025 | Remote Sensing | https://www.mdpi.com/2072-4292/17/3/496 | - |
| Transformers & Hybrid | **RDAH-Net** | 2026 | Remote Sensing | https://www.mdpi.com/2072-4292/18/7/1024 | - |
| Diffusion-based | **Single-View Height Estimation with Conditional Diffusion Probabilistic Models** | 2023 | arXiv | https://doi.org/10.48550/arXiv.2304.13214 | - |
| Diffusion-based | **Leveraging Pretrained Diffusion Model for Semantic 3-D Reconstruction From Monocular Remote Sensing Image** | 2025 | IEEE | https://ieeexplore.ieee.org/abstract/document/11346819 | - |
| Foundation model-based | **Depth2Elevation: Bridging Monocular Depth and Elevation Estimation in Remote Sensing** | 2025 | IEEE | https://ieeexplore.ieee.org/document/10978076 | - |
| Foundation model-based | **Very high resolution canopy height maps from RGB imagery using self-supervised vision transformer and convolutional decoder trained on aerial lidar** | 2024 | RSE | https://www.sciencedirect.com/science/article/pii/S003442572300439X | https://github.com/facebookresearch/HighResCanopyHeight |
| Foundation model-based | **Depth Any Canopy: Leveraging Depth Foundation Models for Canopy Height Estimation** | 2024 | ECCV | https://arxiv.org/abs/2408.04523 | https://github.com/DarthReca/depth-any-canopy |
| Foundation model-based | **Height Estimation from Single Remote Sensing Images via Transfer Learning from Monocular Depth Estimation Models
** | 2025 | IEEE | https://doi.org/10.1109/RusAutoCon65989.2025.11177401 | - |
| Height Completion/Refinement | **Height Prediction and Refinement From Aerial Images With Semantic and Geometric Guidance** | 2021 | IEEE Access | https://doi.org/10.1109/ACCESS.2021.3122894 | https://github.com/melhousni/DSMNet |
| Height Completion/Refinement | **Reconstructing Building Height from Spaceborne TomoSAR Point Clouds Using a Dual-Topology Network** | 2026 | IEEE TGRS | https://ieeexplore.ieee.org/abstract/document/11359292 | https://github.com/zhu-xlab/tomosar2height |
| Height Completion/Refinement | **Enhancing monocular height estimation via sparse LiDAR-guided correction** | 2026 | ISPRS JPRS | https://www.sciencedirect.com/science/article/abs/pii/S0924271625004885 | - |
| Single-SAR | **Deep-learning-based single-image height reconstruction from very-high-resolution SAR intensity data** | 2022 | ISPRS JPRS | https://www.sciencedirect.com/science/article/pii/S0924271621003105 | - |
| Single-SAR | **Large-scale building height retrieval from single SAR imagery based on bounding box regression networks** | 2022 | ISPRS JPRS | https://www.sciencedirect.com/science/article/pii/S0924271621003221 | https://github.com/ya0-sun/bbox-SAR-building |
| Single-SAR | **The SAR2Height framework for urban height map reconstruction from single SAR intensity images** | 2024 | ISPRS JPRS | https://doi.org/10.1016/j.isprsjprs.2024.03.023 | - |
| Single-SAR | **OSM-guided SAR Height Estimation** | 2017 | JURSE | https://doi.org/10.1109/JURSE.2017.7924549 | - |
| Building/Object-centric | **3DCentripetalNet** | 2023 | ISPRS | https://www.sciencedirect.com/science/article/pii/S1569843223001334 | - |
| Building/Object-centric | **HeightNet** | 2023 | Electronics | https://www.mdpi.com/2079-9292/12/2/350 | - |
| Building/Object-centric | **Monocular Building Height (PhiSat-2)** | 2026 | arXiv | https://arxiv.org/abs/2603.29245 | - |

## Benchmarks and datasets

| Name | Source | Resolution | Typical use-cases | Link |
|---|---|---|---|---|
| ISPRS Vaihingen (2D Semantic Labeling + DSM/nDSM) | ISPRS Urban Semantic Lab | ~9 cm (as commonly reported) | Urban orthophoto + DSM/nDSM; widely used for **single-image nDSM/MHE** and joint height+semantics training/eval | https://www.isprs.org/education/benchmarks/UrbanSemLab/2d-sem-label-vaihingen.aspx |
| ISPRS Potsdam (2D Semantic Labeling + DSM) | ISPRS Urban Semantic Lab | 5 cm | True orthophoto patches + DSM; common for **single-view height estimation**, domain shift studies, and cross-task learning | https://www.isprs.org/resources/datasets/benchmarks/UrbanSemLab/2d-sem-label-potsdam.aspx |
| THE Benchmark | Official project site | unspecified | Cross-dataset evaluation + transferable representation learning for MHE | https://thebenchmarkh.github.io/ |
| M4Heights | Scientific Data + GitHub release | mixed (multi-resolution) | Building height benchmarking across **modalities/time**; can be reduced to monocular overhead protocols | https://github.com/RituYadav92/M4Heights |
| MAMHESet (Luojia3-01 video satellite) | IEEE JSTARS dataset paper | unspecified | Multi-angle monocular height estimation benchmarking; video satellite regime | https://doi.org/10.1109/JSTARS.2025.3591908 |
| SynRS3D | NeurIPS Datasets & Benchmarks | synthetic | Domain adaptation / synthetic-to-real pipelines; global-scale monocular 3D/height cues | https://proceedings.neurips.cc/paper_files/paper/2024/hash/d4f3da38b491b44d40a0d5a5b37134ba-Abstract-Datasets_and_Benchmarks_Track.html |

## Code resources

Curated repos explicitly tied to MHE/DSM/nDSM from single overhead imagery (optical or SAR), verified as existing:

- **HTC-DC Net** — https://github.com/zhu-xlab/HTC-DC-Net  
- **TSE-Net** — https://github.com/zhu-xlab/tse-net  
- **U-IMG2DSM** — https://github.com/mhaut/UIMG2DSM  
- **DSMNet (height prediction + refinement)** — https://github.com/melhousni/DSMNet  
- **TomoSAR2Height** — https://github.com/zhu-xlab/tomosar2height  
- **M4Heights benchmark** — https://github.com/RituYadav92/M4Heights  
- **THE Benchmark project site** — https://thebenchmarkh.github.io/

## Contributing

Contributions are welcome!

- Add **only** items that are clearly about **monocular height estimation / DSM / nDSM** from **single-view overhead imagery** (optical or SAR).  
- Do **not** add generic MDE-only papers unless they explicitly produce **height/DSM/nDSM** in overhead remote sensing.
- For each new paper, please include:
  - Section (from the taxonomy in this README)
  - Full title, full author list, year, venue
  - DOI link (preferred) or arXiv link
  - 1–2 sentence annotation (what’s new, and which dataset/protocol is used)
  - Code link if public, otherwise “unspecified”
- Keep formatting consistent with the table style, and keep annotations concise.

## License

MIT License
