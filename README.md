# Awesome Monocular Height Estimation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of papers, datasets, benchmarks, and tools for **Monocular Height Estimation (MHE)** and **single-view DSM/nDSM reconstruction** from overhead imagery.

---

## 📚 CNN / Encoder-Decoder Methods

| Title | Year | Paper | Code | Description |
|------|------|------|------|------------|
| IM2HEIGHT | 2018 | https://arxiv.org/abs/1802.10249 | - | First deep CNN for dense height regression from aerial imagery |
| IMG2DSM | 2018 | - | - | GAN-based DSM generation from RGB imagery |
| Joint Height + Semantics CNN | 2017 | https://ieeexplore.ieee.org/document/8128167 | - | Multi-task learning improves structural consistency |
| ISPRS CNN Baseline | 2019 | https://www.sciencedirect.com/science/article/pii/S0924271619300139 | - | Strong encoder-decoder baseline widely reused |
| IM2ELEVATION | 2020 | https://www.mdpi.com/2072-4292/12/17/2719 | - | Large-scale supervised DSM prediction |
| Ordinal Regression MHE | 2020 | https://arxiv.org/abs/2006.02801 | - | Reformulates regression as classification |
| IMG2nDSM | 2021 | https://www.mdpi.com/2072-4292/13/12/2417 | - | Focuses on normalized DSM prediction |
| Mask-Height R-CNN | 2021 | https://ieeexplore.ieee.org/document/9553121 | - | Instance-level height estimation |
| Shadow-guided CNN | 2021 | https://arxiv.org/abs/2104.10874 | - | Uses shadows explicitly in deep learning |
| Street-view + Aerial | 2023 | https://arxiv.org/pdf/2311.02121 | - | Cross-view supervision improves MHE |
| LUMNet | 2024 | - | - | Land-use guided multi-scale network |
| RDAH-Net | 2026 | https://www.mdpi.com/2072-4292/18/7/1024 | - | Bridges relative depth and absolute height |

---

## 🔷 Transformers & Hybrid Methods

| Title | Year | Paper | Code | Description |
|------|------|------|------|------------|
| THE Benchmark | 2021 | https://arxiv.org/abs/2112.14985 | https://thebenchmarkh.github.io/ | First cross-dataset benchmark |
| HTC-DC Net | 2023 | https://arxiv.org/abs/2309.16486 | - | CNN + Transformer fusion for MHE |
| HeightFormer | 2024 | https://arxiv.org/abs/2310.07995 | - | Multi-scale transformer with global context |
| CMT-based MHE | 2025 | https://www.sciencedirect.com/science/article/pii/S0924271625002710 | - | CNN-transformer hybrid improves spatial consistency |
| CNN + ViT Fusion | 2025 | https://openaccess.thecvf.com/... | - | Hybrid encoder improves representation |

---

## 🌫 Diffusion-Based Methods

| Title | Year | Paper | Code | Description |
|------|------|------|------|------------|
| Diffusion MHE | 2023 | https://arxiv.org/abs/2304.13214 | - | Models height estimation as generative process |
| IEEE Diffusion MHE | 2025 | https://ieeexplore.ieee.org/abstract/document/11346819 | - | Adds uncertainty modeling via diffusion |

---

## 📡 SAR-based Height Estimation

| Title | Year | Paper | Code | Description |
|------|------|------|------|------------|
| SAR Height Reconstruction | 2022 | https://www.sciencedirect.com/science/article/pii/S0924271621003105 | - | First DL framework using SAR |
| SAR2Height | 2024 | https://www.sciencedirect.com/science/article/pii/S0924271624000959 | - | Combines geometry + learning |
| Object-based SAR MHE | 2025 | https://arxiv.org/abs/2507.08096 | - | Instance-level SAR height estimation |

---

## 🏢 Object / Building Height Estimation

| Title | Year | Paper | Code | Description |
|------|------|------|------|------------|
| 3DCentripetalNet | 2023 | https://www.sciencedirect.com/... | - | Predicts building height via geometric centers |
| HeightNet | 2023 | https://www.mdpi.com/2079-9292/12/2/350 | - | Object-level height regression |

---

## 📊 Benchmarks & Datasets

| Dataset | Year | Link | Description |
|--------|------|------|------------|
| THE Benchmark | 2021 | https://thebenchmarkh.github.io/ | Cross-dataset generalization |
| MAMHESet | 2025 | - | Multi-angle satellite dataset |
| M4Heights | 2026 | https://www.nature.com/articles/s41597-025-06495-3 | Large-scale benchmark |
| ISPRS Vaihingen | - | - | Standard DSM dataset |
| ISPRS Potsdam | - | - | High-res aerial benchmark |
| DFC2019 | 2019 | - | IEEE GRSS challenge |
| GBH | - | - | Used in HTC-DC Net |

---

## 📏 Evaluation Metrics

| Metric | Description |
|------|------------|
| MAE | Mean Absolute Error |
| RMSE | Root Mean Square Error |
| Per-building RMSE | Instance-level accuracy |
| Boundary Accuracy | Structural quality |
| Cross-domain gap | Generalization ability |

---

## 📄 License

MIT License
