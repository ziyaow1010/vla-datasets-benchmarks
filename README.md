# VLA Datasets & Benchmarks (Vision-Language-Action)

A curated list of datasets and benchmarks for **Vision-Language-Action (VLA)** research.  
This repository focuses on **data formats, evaluation protocols, and benchmark comparability**, with practical guidance on **which dataset/benchmark to use** for different research needs.

> Maintained by: *Ziyao Wang, Bingying Wang, Hanrong Zhang / UMD CaseLab*  
> Scope: datasets + benchmarks + evaluation protocols (no model architecture deep dive)

---

## Table of Contents
- [How to Use This List](#how-to-use-this-list)
- [Tag Legend](#tag-legend)
- [Datasets](#datasets)
  - [Real-World Robot Datasets](#real-world-robot-datasets)
  - [Simulation and Synthetic Datasets](#simulation-and-synthetic-datasets)
  - [Multimodal / Tactile / Special Embodiments](#multimodal--tactile--special-embodiments)
- [Benchmarks](#benchmarks)
  - [Tabletop + Simple Tasks](#tabletop--simple-tasks)
  - [Tabletop + Long-Horizon / Complex Tasks](#tabletop--long-horizon--complex-tasks)
  - [Multi-Scene + Simple Tasks](#multi-scene--simple-tasks)
  - [Multi-Scene + Long-Horizon / Complex Tasks](#multi-scene--long-horizon--complex-tasks)
- [Evaluation Protocols & Metrics](#evaluation-protocols--metrics)
- [Contributing](#contributing)
- [Citation](#citation)

---

## How to Use This List
This repository is organized to answer three practical questions:

1. **What exists?** What datasets and benchmarks are commonly used in VLA research?  
2. **How are they used?** What are the key data formats, action representations, task setups, and evaluation protocols?  
3. **Which should I choose?** Given a research goal (e.g., long-horizon tasks, OOD generalization, sim-to-real), which datasets or benchmarks best match the need?

We keep each entry short and rely on **colored tags** (badges) to highlight key properties.

---

## Tag Legend

### Dataset tags
**Dataset type**
- ![](https://img.shields.io/badge/ds--real-2ea44f) real robot data
- ![](https://img.shields.io/badge/ds--synthetic-8957e5) synthetic or simulation-generated data
- ![](https://img.shields.io/badge/ds--mixed-8b949e) mixed real + synthetic (or mixed sources)

**Action representation**
- ![](https://img.shields.io/badge/act--delta-1f6feb) delta (incremental) actions
- ![](https://img.shields.io/badge/act--absolute-0a3069) absolute actions
- ![](https://img.shields.io/badge/act--mixed-8b949e) mixed / heterogeneous actions

**Control target**
- ![](https://img.shields.io/badge/ctrl--EEF-f85149) end-effector (EEF) control
- ![](https://img.shields.io/badge/ctrl--DoF-d29922) joint (DoF) control
- ![](https://img.shields.io/badge/ctrl--mixed-8b949e) mixed / heterogeneous control targets

**Vision modality**
- ![](https://img.shields.io/badge/vis--image-0ea5e9) image
- ![](https://img.shields.io/badge/vis--3D-14b8a6) 3D (RGB-D / point cloud)
- ![](https://img.shields.io/badge/vis--video-0284c7) video

### Shared task tags (datasets + benchmarks)
- ![](https://img.shields.io/badge/task--tabletop-f59e0b) tabletop
- ![](https://img.shields.io/badge/task--multi--scene-d29922) multi-scene
- ![](https://img.shields.io/badge/task--short-0ea5e9) short-horizon
- ![](https://img.shields.io/badge/task--long-ec4899) long-horizon

---

# Datasets

## Real-World Robot Datasets

- **Benchmarking Vision, Language, & Action Models on Robotic Learning Tasks, (2023, arXiv)** Pranav Guruprasad, Harshvardhan Sikka, Jaewoo Song, Yangyue Wang, Paul Pu Liang
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper](https://ieeexplore.ieee.org/document/10611477) | [website]() | [code]()

- **RT-1 Dataset (2022, arXiv)** 
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--delta-1f6feb) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

- **RT-2 Data (2023, arXiv)** 
![](https://img.shields.io/badge/ds--mixed-8b949e) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--image-0ea5e9)  
Links: [paper]() | [website]() | [code]()

- **DROID (2024, RSS)** 
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--delta-1f6feb) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--tabletop-f59e0b)  
Links: [paper]() | [website]() | [code]()

- **BridgeData V2 (2023, CoRL)** 
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--delta-1f6feb) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--3D-14b8a6) ![](https://img.shields.io/badge/task--tabletop-f59e0b)  
Links: [paper]() | [website]() | [code]()

- **RH20T (2023, RSS)** 
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--absolute-0a3069) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--3D-14b8a6) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper]() | [website]() | [code]()

- **Ego4D (2022, CVPR)** 
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--absolute-0a3069) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--video-0284c7) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper]() | [website]() | [code]()

> Note: Ego4D is a human egocentric video dataset (no robot actions), often used for learning visual affordances and priors.

---

## Simulation and Synthetic Datasets

- **GraspVLA (2025, arXiv)** 
![](https://img.shields.io/badge/ds--synthetic-8957e5) ![](https://img.shields.io/badge/act--absolute-0a3069) ![](https://img.shields.io/badge/ctrl--DoF-d29922) ![](https://img.shields.io/badge/vis--3D-14b8a6) ![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

- **RoboGen (2024, ICML)** 
![](https://img.shields.io/badge/ds--synthetic-8957e5) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper]() | [website]() | [code]()

- **MimicGen (2023, CoRL)** 
![](https://img.shields.io/badge/ds--synthetic-8957e5) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--tabletop-f59e0b)  
Links: [paper]() | [website]() | [code]()

---

## Multimodal / Tactile / Special Embodiments
(You can add more datasets here later, e.g., tactile datasets, bimanual datasets, mobile manipulation.)

---

# Benchmarks

## Tabletop + Simple Tasks
Short-horizon tabletop manipulation benchmarks under controlled settings.

- **Meta-World (2021, arXiv)** 
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

- **LIBERO (2023, CoRL)** 
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

- **SimplerEnv (2024, arXiv)** 
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

---

## Tabletop + Long-Horizon / Complex Tasks
Long-horizon instruction following and compositional manipulation in tabletop settings.

- **CALVIN (2022, arXiv)** 
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper]() | [website]() | [code]()

---

## Multi-Scene + Simple Tasks
(Reserved. Add representative benchmarks when needed.)

---

## Multi-Scene + Long-Horizon / Complex Tasks
Multi-room / full-scene environments with long-horizon and compositional tasks.

- **BEHAVIOR-1K (2024)** 
![](https://img.shields.io/badge/task--multi--scene-d29922) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper]() | [website]() | [code]()

- **VLABench (2024, arXiv)** 
![](https://img.shields.io/badge/task--multi--scene-d29922) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper]() | [website]() | [code]()

- **Open X-Embodiment (Evaluation Regime)** 
![](https://img.shields.io/badge/task--multi--scene-d29922) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper]() | [website]() | [code]()

---

# Evaluation Protocols & Metrics
Common factors that affect benchmark comparability:

- **Success criteria:** binary success vs graded progress  
- **Reset policy:** scripted resets vs human resets vs autonomous resets  
- **Generalization splits:** object OOD vs scene OOD vs task OOD (definitions vary)  
- **Embodiment shift:** evaluation across robots with different DoF and action spaces  
- **Reporting:** number of seeds, number of tasks, confidence intervals  

---

## Contributing
We welcome contributions.

### Add a new entry (short format)

```text
Name (Year, Venue):
Tags: [ds-real/ds-synthetic/ds-mixed] [act-delta/act-absolute] [ctrl-EEF/ctrl-DoF] [vis-image/vis-3D/vis-video] [task-tabletop/multi-scene] [task-short/long]
Links: paper | website | code
