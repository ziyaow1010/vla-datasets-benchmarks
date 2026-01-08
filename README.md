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

- **Benchmarking Vision, Language, & Action Models on Robotic Learning Tasks (2023, arXiv)**
  Pranav Guruprasad, Harshvardhan Sikka, Jaewoo Song, Yangyue Wang, Paul Pu Liang
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper](https://ieeexplore.ieee.org/document/10611477) | [website]() | [code]()

- **RT-1: Robotics Transformer for Real-World Control at Scale (2022, arXiv)**
  Anthony Brohan, Noah Brown, Justice Carbajal et al.
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--delta-1f6feb) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper](https://arxiv.org/pdf/2212.06817) | [website]() | [code]()

- **RT-2: Vision-Language-Action Models Transfer Web Knowledge to Robotic Control (2023, PMLR)**
  Brianna Zitkovich, Tianhe Yu, Sichun Xu et al.
![](https://img.shields.io/badge/ds--mixed-8b949e) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--image-0ea5e9)  
Links: [paper](https://proceedings.mlr.press/v229/zitkovich23a/zitkovich23a.pdf) | [website](https://proceedings.mlr.press/v229/zitkovich23a.html) | [code]()

- **DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset (2024, RSS)**
  Alexander Khazatsky, Karl Pertsch, Suraj Nair et al.
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--delta-1f6feb) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--tabletop-f59e0b)  
Links: [paper](https://arxiv.org/pdf/2403.12945) | [website]() | [code]()

- **BridgeData V2: A Dataset for Robot Learning at Scale (2023, PMLR)**
  Homer Rich Walke, Kevin Black, Tony Z. Zhao, Quan Vuong, Chongyi Zheng, Philippe Hansen-Estruch, Andre Wang He, Vivek Myers, Moo Jin Kim, Max Du, Abraham Lee, Kuan Fang, Chelsea Finn, Sergey Levine
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--delta-1f6feb) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--3D-14b8a6) ![](https://img.shields.io/badge/task--tabletop-f59e0b)  
Links: [paper](https://proceedings.mlr.press/v229/walke23a/walke23a.pdf) | [website]() | [code]()

- **RH20T: A Comprehensive Robotic Dataset for Learning Diverse Skills in One-Shot (2023, RSS)**
  Hao-Shu Fang, Hongjie Fang, Zhenyu Tang, Jirong Liu, Chenxi Wang, Junbo Wang, Haoyi Zhu, Cewu Lu
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--absolute-0a3069) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--3D-14b8a6) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper](https://arxiv.org/pdf/2307.00595) | [website]() | [code]()

- **Ego4D: Around the World in 3,000 Hours of Egocentric Video (2022, CVPR)**
  Kristen Grauman, Andrew Westbury, Eugene Byrne et al.
![](https://img.shields.io/badge/ds--real-2ea44f) ![](https://img.shields.io/badge/act--absolute-0a3069) ![](https://img.shields.io/badge/ctrl--EEF-f85149) ![](https://img.shields.io/badge/vis--video-0284c7) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper](https://openaccess.thecvf.com/content/CVPR2022/papers/Grauman_Ego4D_Around_the_World_in_3000_Hours_of_Egocentric_Video_CVPR_2022_paper.pdf) | [website]() | [code]()

> Note: Ego4D is a human egocentric video dataset (no robot actions), often used for learning visual affordances and priors.

---

## Simulation and Synthetic Datasets

- **GraspVLA: a Grasping Foundation Model Pre-trained on Billion-scale Synthetic Action Data (2025, arXiv)**
  Shengliang Deng, Mi Yan, Songlin Wei, Haixin Ma, Yuxin Yang, Jiayi Chen, Zhiqi Zhang, Taoyu Yang, Xuheng Zhang, Wenhao Zhang, Heming Cui, Zhizheng Zhang, He Wang
![](https://img.shields.io/badge/ds--synthetic-8957e5) ![](https://img.shields.io/badge/act--absolute-0a3069) ![](https://img.shields.io/badge/ctrl--DoF-d29922) ![](https://img.shields.io/badge/vis--3D-14b8a6) ![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper](https://arxiv.org/pdf/2505.03233) | [website]() | [code]()

- **RoboGen: Towards Unleashing Infinite Data for Automated Robot Learning via Generative Simulation (2024, ICML)**
  Yufei Wang, Zhou Xian, Feng Chen, Tsun-Hsuan Wang, Yian Wang, Katerina Fragkiadaki, Zackory Erickson, David Held, Chuang Gan
![](https://img.shields.io/badge/ds--synthetic-8957e5) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--multi--scene-d29922)  
Links: [paper](https://arxiv.org/pdf/2311.01455) | [website]() | [code]()

- **MimicGen: A Data Generation System for Scalable Robot Learning using Human Demonstrations (2023, CoRL)**
  Ajay Mandlekar, Soroush Nasiriany, Bowen Wen, Iretiayo Akinola, Yashraj Narang, Linxi Fan, Yuke Zhu, Dieter Fox
![](https://img.shields.io/badge/ds--synthetic-8957e5) ![](https://img.shields.io/badge/act--mixed-8b949e) ![](https://img.shields.io/badge/ctrl--mixed-8b949e) ![](https://img.shields.io/badge/vis--image-0ea5e9) ![](https://img.shields.io/badge/task--tabletop-f59e0b)  
Links: [paper](https://arxiv.org/pdf/2310.17596) | [website]() | [code]()

---

## Multimodal / Tactile / Special Embodiments
(You can add more datasets here later, e.g., tactile datasets, bimanual datasets, mobile manipulation.)

---

# Benchmarks

## Tabletop + Simple Tasks
Short-horizon tabletop manipulation benchmarks under controlled settings.

- **Meta-World: A Benchmark and Evaluation for Multi-Task and Meta Reinforcement Learning (2021, arXiv)**
  Tianhe Yu, Deirdre Quillen, Zhanpeng He, Ryan Julian, Karol Hausman, Chelsea Finn, Sergey Levine
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper](https://proceedings.mlr.press/v100/yu20a/yu20a.pdf) | [website]() | [code]()

- **LIBERO: Benchmarking Knowledge Transfer for Lifelong Robot Learning (2023, NeurIPS)**
  Bo Liu, Yifeng Zhu, Chongkai Gao, Yihao Feng, Qiang Liu, Yuke Zhu, Peter Stone
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper](https://proceedings.neurips.cc/paper_files/paper/2023/file/8c3c666820ea055a77726d66fc7d447f-Paper-Datasets_and_Benchmarks.pdf) | [website]() | [code]()

- **Evaluating Real-World Robot Manipulation Policies in Simulation (2024, arXiv)**
  Xuanlin Li, Kyle Hsu, Jiayuan Gu, Karl Pertsch, Oier Mees, Homer Rich Walke, Chuyuan Fu, Ishikaa Lunawat, Isabel Sieh, Sean Kirmani, Sergey Levine, Jiajun Wu, Chelsea Finn, Hao Su, Quan Vuong, Ted Xiao
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--short-0ea5e9)  
Links: [paper](https://arxiv.org/pdf/2405.05941) | [website]() | [code]()

---

## Tabletop + Long-Horizon / Complex Tasks
Long-horizon instruction following and compositional manipulation in tabletop settings.

- **CALVIN: A Benchmark for Language-Conditioned Policy Learning for Long-Horizon Robot Manipulation Tasks (2022, arXiv)**
  Oier Mees, Lukas Hermann, Erick Rosete-Beas, Wolfram Burgard
![](https://img.shields.io/badge/task--tabletop-f59e0b) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper](https://arxiv.org/pdf/2112.03227) | [website]() | [code]()

---

## Multi-Scene + Simple Tasks
(Reserved. Add representative benchmarks when needed.)

---

## Multi-Scene + Long-Horizon / Complex Tasks
Multi-room / full-scene environments with long-horizon and compositional tasks.

- **BEHAVIOR-1K: A Benchmark for Embodied AI with 1,000 Everyday Activities and Realistic Simulation (2024)**
  Chengshu Li, Ruohan Zhang, Josiah Wong, Cem Gokmen, Sanjana Srivastava, Roberto Martín-Martín, Chen Wang, Gabrael Levine, Michael Lingelbach, Jiankai Sun, Mona Anvari, Minjune Hwang, Manasi Sharma, Arman Aydin, Dhruva Bansal, Samuel Hunter, Kyu-Young Kim, Alan Lou, Caleb R Matthews, Ivan Villa-Renteria, Jerry Huayang Tang, Claire Tang, Fei Xia, Silvio Savarese, Hyowon Gweon, Karen Liu, Jiajun Wu, Li Fei-Fei
![](https://img.shields.io/badge/task--multi--scene-d29922) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper](https://proceedings.mlr.press/v205/li23a/li23a.pdf) | [website]() | [code]()

- **VLABench: A Large-Scale Benchmark for Language-Conditioned Robotics Manipulation with Long-Horizon Reasoning Tasks (2024, arXiv)**
  Shiduo Zhang, Zhe Xu, Peiju Liu, Xiaopeng Yu, Yuan Li, Qinghui Gao, Zhaoye Fei, Zhangyue Yin, Zuxuan Wu, Yu-Gang Jiang, Xipeng Qiu
![](https://img.shields.io/badge/task--multi--scene-d29922) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper](https://openaccess.thecvf.com/content/ICCV2025/papers/Zhang_VLABench_A_Large-Scale_Benchmark_for_Language-Conditioned_Robotics_Manipulation_with_Long-Horizon_ICCV_2025_paper.pdf) | [website]() | [code]()

- **Open X-Embodiment: Robotic Learning Datasets and RT-X Models (Evaluation Regime)**
  Open X-Embodiment Collaboration et al.
![](https://img.shields.io/badge/task--multi--scene-d29922) ![](https://img.shields.io/badge/task--long-ec4899)  
Links: [paper](https://arxiv.org/pdf/2310.08864) | [website]() | [code]()

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
