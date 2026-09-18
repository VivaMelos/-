# Awesome Virtual Cell Literature

面向课程综述和虚拟细胞挑战赛的文献仓库。结构参考 `Awesome-Virtual-Spatial-Omics-Generation`，但主题从“病理图像到空间组学生成”改为：

**AI虚拟细胞、单细胞扰动响应预测、细胞状态建模、基础模型与benchmark。**

## Overview

虚拟细胞的目标不是简单复现一个细胞图像，而是构建能够预测细胞状态变化的计算模型。对你当前综述来说，最核心的分支是：

> 单细胞扰动响应预测：给定细胞类型、初始状态和扰动条件，预测扰动后的转录组或细胞状态。

典型扰动包括基因敲除、基因敲低、基因过表达、CRISPR扰动、药物处理和组合扰动。

## Table of Contents

- [Papers](#papers)
  - [Roadmap, Survey and Perspective](#roadmap-survey-and-perspective)
  - [Benchmark and Challenge](#benchmark-and-challenge)
  - [Perturbation Data and Experimental Platform](#perturbation-data-and-experimental-platform)
  - [Perturbation Response Prediction Models](#perturbation-response-prediction-models)
  - [Single-Cell Foundation Models](#single-cell-foundation-models)
  - [Virtual Spatial and Multi-Omics Generation](#virtual-spatial-and-multi-omics-generation)
- [How to Use This Repository](#how-to-use-this-repository)
- [Local Notes](#local-notes)

## Papers

### Roadmap, Survey and Perspective

| Year | Title | Venue | Field | Paper |
|---:|---|---|---|---|
| 2026 | Towards an AI co-scientist: Cellular perturbation foundation models for biomolecular discovery | Frontiers in Artificial Intelligence | Perspective | [link](https://www.frontiersin.org/journals/artificial-intelligence/articles/10.3389/frai.2026.1713891/full) |
| 2026 | Toward trustworthy virtual cells: Interpretability, multiscale modelling, and therapeutic discovery | arXiv | Perspective | [link](https://arxiv.org/abs/2608.14258) |
| 2026 | The virtual cell challenge | NeurIPS Workshop / arXiv | Challenge overview | [link](https://arxiv.org/abs/2609.05413) |
| 2024 | AI Virtual Cell | Chan Zuckerberg Initiative | Research program | [link](https://chanzuckerberg.com/science/programs-resources/single-cell-biology/ai-virtual-cell/) |

### Benchmark and Challenge

| Year | Title | Organizer / Venue | Task | Paper / Website | Code |
|---:|---|---|---|---|---|
| 2026 | Virtual Cell Challenge | Arc Institute / NVIDIA | Predict single-cell perturbation responses in unseen contexts | [link](https://virtualcellchallenge.org/) | [starter kit](https://github.com/ArcInstitute/state) |
| 2026 | State: A virtual cell model for in silico perturbation biology | Cell | Virtual cell model and VCC baseline direction | [link](https://www.cell.com/cell/fulltext/S0092-8674(26)00987-4) | [code](https://github.com/ArcInstitute/state) |
| 2026 | Myllia Echoes: Predicting cellular perturbations across contexts | Kaggle / Arc Institute | Challenge dataset and leaderboard | [link](https://www.kaggle.com/competitions/myllia-echoes) | - |
| 2026 | Benchmarking algorithms for predicting cellular responses to perturbation | Nature Methods | Systematic benchmark | [link](https://www.nature.com/articles/s41592-026-03490-3) | - |

### Perturbation Data and Experimental Platform

| Year | Title | Venue | Field | Paper | Code / Data |
|---:|---|---|---|---|---|
| 2016 | Perturb-seq: Dissecting molecular circuits with scalable single-cell RNA profiling of pooled genetic screens | Cell | Perturb-seq | [link](https://www.cell.com/cell/fulltext/S0092-8674(16)31611-7) | - |
| 2016 | CRISP-seq: Single-cell transcriptomic analysis of CRISPR-mediated genetic perturbation | Cell | CRISPR + scRNA-seq | [link](https://www.cell.com/cell/fulltext/S0092-8674(16)31610-5) | - |
| 2019 | Exploring genetic interaction manifolds constructed from rich single-cell phenotypes | Science | Combinatorial perturbation | [link](https://www.science.org/doi/10.1126/science.aax4438) | [data](https://github.com/theislab/sc-pert) |
| 2022 | Mapping information-rich genotype-phenotype landscapes with genome-scale Perturb-seq | Cell | Genome-scale Perturb-seq | [link](https://www.cell.com/cell/fulltext/S0092-8674(22)00597-9) | - |

### Perturbation Response Prediction Models

| Year | Title | Venue | Method | Task | Paper | Code |
|---:|---|---|---|---|---|---|
| 2019 | scGen predicts single-cell perturbation responses | Nature Methods | VAE / latent arithmetic | Perturbation prediction | [link](https://www.nature.com/articles/s41592-019-0494-8) | [code](https://github.com/theislab/scgen) |
| 2023 | Predicting cellular responses to complex perturbations in high-throughput screens | Molecular Systems Biology | Compositional Perturbation Autoencoder | Genetic / drug perturbation | [link](https://www.embopress.org/doi/full/10.15252/msb.202211517) | [code](https://github.com/theislab/cpa) |
| 2023 | Learning single-cell perturbation responses using neural optimal transport | Nature Methods | CellOT | Distribution-level perturbation prediction | [link](https://www.nature.com/articles/s41592-023-01969-x) | [code](https://github.com/bunnech/cellot) |
| 2023 | Predicting transcriptional outcomes of novel multigene perturbations with GEARS | Nature Biotechnology | Graph neural network | Unseen and combinatorial perturbation | [link](https://www.nature.com/articles/s41587-023-01905-6) | [code](https://github.com/snap-stanford/GEARS) |
| 2023 | CellOracle: Dissecting cell identity via network-based in silico gene perturbation | Nature | Gene regulatory network simulation | In silico gene perturbation | [link](https://www.nature.com/articles/s41586-022-05688-9) | [code](https://github.com/morris-lab/CellOracle) |
| 2026 | State: A virtual cell model for in silico perturbation biology | Cell | Virtual cell model | Challenge-scale perturbation prediction | [link](https://www.cell.com/cell/fulltext/S0092-8674(26)00987-4) | [code](https://github.com/ArcInstitute/state) |

### Single-Cell Foundation Models

| Year | Title | Venue | Method | Main Use | Paper | Code |
|---:|---|---|---|---|---|---|
| 2023 | Transfer learning enables predictions in network biology | Nature | Geneformer | Gene / cell representation, perturbation-related prediction | [link](https://www.nature.com/articles/s41586-023-06139-9) | [code](https://huggingface.co/ctheodoris/Geneformer) |
| 2024 | scGPT: Toward building a foundation model for single-cell multi-omics using generative AI | Nature Methods | Transformer / generative pretraining | Cell embedding and multi-task single-cell analysis | [link](https://www.nature.com/articles/s41592-024-02201-0) | [code](https://github.com/bowang-lab/scGPT) |
| 2024 | Large-scale foundation model on single-cell transcriptomics | Nature Methods | scFoundation | General single-cell representation | [link](https://www.nature.com/articles/s41592-024-02305-7) | [code](https://github.com/biomap-research/scFoundation) |
| 2024 | Universal Cell Embeddings: A foundation model for cell biology | bioRxiv | Universal cell embedding | Cell representation across datasets | [link](https://www.biorxiv.org/content/10.1101/2023.11.28.568918v2) | - |
| 2026 | CellFM: A large-scale foundation model pretrained on transcriptomics of 100 million human cells | bioRxiv | Cell foundation model | General virtual-cell representation | [link](https://www.biorxiv.org/content/10.1101/2026.01.07.575156v1) | - |

### Virtual Spatial and Multi-Omics Generation

这一类不是你综述的主线，但可以作为“虚拟细胞/虚拟组织”的相邻方向。参考仓库 `Awesome-Virtual-Spatial-Omics-Generation` 主要收集的就是这个方向。

| Year | Title | Venue | Direction | Paper | Code |
|---:|---|---|---|---|---|
| 2020 | Integrating spatial gene expression and breast tumour morphology via deep learning | Nature Biomedical Engineering | H&E to spatial transcriptomics | [link](https://www.nature.com/articles/s41551-020-0578-x) | [code](https://github.com/bryanhe/ST-Net) |
| 2022 | Spatial transcriptomics prediction from histology jointly through transformer and graph neural networks | Briefings in Bioinformatics | H&E to spatial transcriptomics | [link](https://doi.org/10.1093/bib/bbac297) | [code](https://github.com/biomed-AI/Hist2ST) |
| 2024 | Digital profiling of gene expression from histology images with linearized attention | Nature Communications | WSI to gene expression | [link](https://www.nature.com/articles/s41467-024-54182-5) | [code](https://github.com/gevaertlab/sequoia-pub) |
| 2025 | Spatially resolved gene expression prediction from histology images via bi-modal contrastive learning | NeurIPS | H&E to spatial transcriptomics | [link](https://arxiv.org/pdf/2306.01859) | [code](https://github.com/bowang-lab/BLEEP) |
| 2026 | H2O: A Foundation Model Bridging Histopathology to Spatial Multi-Omics Profiling | bioRxiv | H&E to spatial multi-omics | [link](https://www.biorxiv.org/content/10.64898/2026.04.21.717342v1) | [code](https://github.com/TencentAILabHealthcare/H2O) |

## How to Use This Repository

建议按下面顺序读：

1. 先读 `Roadmap, Survey and Perspective`，明确“虚拟细胞”的大背景。
2. 再读 `Perturbation Data and Experimental Platform`，理解扰动数据从哪里来。
3. 重点读 `Perturbation Response Prediction Models`，这是综述主线。
4. 补充读 `Single-Cell Foundation Models`，用于解释为什么基础模型可能提升扰动预测。
5. 最后用 `Benchmark and Challenge` 写出你的挑战赛切入点。

## Local Notes

- 综述主线文件：[../综述大纲.md](../综述大纲.md)
- 挑战赛切入点：[../挑战赛切入点.md](../挑战赛切入点.md)
- 文献阅读表：[../文献阅读表.md](../文献阅读表.md)
- 文献卡片模板：[templates/文献卡片模板.md](templates/文献卡片模板.md)

