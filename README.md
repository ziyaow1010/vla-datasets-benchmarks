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

1. **What exists?**  
2. **How are they used?**  
3. **Which should I choose?**

We keep each entry short (a few lines) and rely on **colored tags** to highlight key properties.  
If you are new to VLA, start from:
- **[Tag Legend](#tag-legend)** for quick filtering
- **[Evaluation Protocols & Metrics](#evaluation-protocols--metrics)** for comparability pitfalls

---

## Tag Legend
We use small colored tags (badges) to summarize key properties.

**Data source**
- ![](https://img.shields.io/badge/real-2ea44f) real robot data
- ![](https://img.shields.io/badge/sim-1f6feb) simulation
- ![](https://img.shields.io/badge/synthetic-8957e5) synthetic generation
- ![](https://img.shields.io/badge/web-8b949e) web / egocentric video

**Environment**
- ![](https://img.shields.io/badge/tabletop-f85149) tabletop
- ![](https://img.shields.io/badge/multi--scene-d29922) multi-scene

**Task horizon**
- ![](https://img.shields.io/badge/short-0ea5e9) short-horizon
- ![](https://img.shields.io/badge/long-ec4899) long-horizon

**Scale**
- ![](https://img.shields.io/badge/large--scale-3fb950) large scale
- ![](https://img.shields.io/badge/small--scale-ff7b72) small scale

**Generalization / protocol**
- ![](https://img.shields.io/badge/OOD-ffd33d) OOD splits
- ![](https://img.shields.io/badge/protocol-6e40c9) standardized protocol
- ![](https://img.shields.io/badge/real--eval-2ea44f) real-world evaluation

You can add new tags if needed, but keep the tag set compact.

---

# Datasets

## Real-World Robot Datasets

### **DROID (2023)** ![](https://img.shields.io/badge/real-2ea44f) ![](https://img.shields.io/badge/tabletop-f85149) ![](https://img.shields.io/badge/large--scale-3fb950)  
Links: [paper]() | [website]() | [code]()

### **RH20T (2023)** ![](https://img.shields.io/badge/real-2ea44f) ![](https://img.shields.io/badge/multi--scene-d29922) ![](https://img.shields.io/badge/large--scale-3fb950)  
Links: [paper]() | [website]() | [code]()

### **Open X-Embodiment (2023)** ![](https://img.shields.io/badge/real-2ea44f) ![](https://img.shields.io/badge/multi--robot-6e40c9) ![](https://img.shields.io/badge/large--scale-3fb950)  
Links: [paper]() | [website]() | [code]()

---

## Simulation and Synthetic Datasets

### **RoboNet (2019)** ![](https://img.shields.io/badge/real-2ea44f) ![](https://img.shields.io/badge/multi--robot-6e40c9)  
Links: [paper]() | [website]() | [code]()

### **Meta-World Data (2019)** ![](https://img.shields.io/badge/sim-1f6feb) ![](https://img.shields.io/badge/tabletop-f85149) ![](https://img.shields.io/badge/short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

### **ReBot (2025)** ![](https://img.shields.io/badge/synthetic-8957e5) ![](https://img.shields.io/badge/sim2real-6e40c9) ![](https://img.shields.io/badge/large--scale-3fb950)  
Links: [paper]() | [website]() | [code]()

---

## Multimodal / Tactile / Special Embodiments

### **GelSight / Tactile Dataset (Year)** ![](https://img.shields.io/badge/tactile-6e40c9) ![](https://img.shields.io/badge/real-2ea44f)  
Links: [paper]() | [website]() | [code]()

---

# Benchmarks

## Tabletop + Simple Tasks
Short-horizon tabletop manipulation benchmarks, often used for quick iteration and controlled comparisons.

### **Meta-World (2019)** ![](https://img.shields.io/badge/sim-1f6feb) ![](https://img.shields.io/badge/tabletop-f85149) ![](https://img.shields.io/badge/short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

### **LIBERO (2023)** ![](https://img.shields.io/badge/sim-1f6feb) ![](https://img.shields.io/badge/tabletop-f85149) ![](https://img.shields.io/badge/short-0ea5e9) ![](https://img.shields.io/badge/OOD-ffd33d)  
Links: [paper]() | [website]() | [code]()

### **SimplerEnv (2024)** ![](https://img.shields.io/badge/sim-1f6feb) ![](https://img.shields.io/badge/tabletop-f85149) ![](https://img.shields.io/badge/protocol-6e40c9)  
Links: [paper]() | [website]() | [code]()

---

## Tabletop + Long-Horizon / Complex Tasks
Long-horizon tabletop benchmarks designed to study planning and compounding errors.

### **CALVIN (2021)** ![](https://img.shields.io/badge/sim-1f6feb) ![](https://img.shields.io/badge/tabletop-f85149) ![](https://img.shields.io/badge/long-ec4899) ![](https://img.shields.io/badge/protocol-6e40c9)  
Links: [paper]() | [website]() | [code]()

---

## Multi-Scene + Simple Tasks
Multi-scene benchmarks with relatively simple task structures, usually emphasizing environment variation.

### **Benchmark Name (Year)** ![](https://img.shields.io/badge/multi--scene-d29922) ![](https://img.shields.io/badge/short-0ea5e9)  
Links: [paper]() | [website]() | [code]()

---

## Multi-Scene + Long-Horizon / Complex Tasks
Multi-scene and compositional benchmarks for long-horizon language-conditioned tasks.

### **BEHAVIOR-1K (2022)** ![](https://img.shields.io/badge/sim-1f6feb) ![](https://img.shields.io/badge/multi--scene-d29922) ![](https://img.shields.io/badge/long-ec4899)  
Links: [paper]() | [website]() | [code]()

### **VLABench (2024)** ![](https://img.shields.io/badge/sim-1f6feb) ![](https://img.shields.io/badge/multi--scene-d29922) ![](https://img.shields.io/badge/long-ec4899) ![](https://img.shields.io/badge/OOD-ffd33d)  
Links: [paper]() | [website]() | [code]()

---

# Evaluation Protocols & Metrics
Common sources of inconsistency that make benchmark results hard to compare:

- **Success criteria:** binary success vs graded progress  
- **Reset policy:** scripted resets vs human resets vs autonomous resets  
- **Generalization splits:** object OOD vs scene OOD vs task OOD (definitions vary)  
- **Embodiment shift:** evaluation across robots with different DoF and action spaces  
- **Safety metrics:** collisions, unsafe contact, drop rates  
- **Reporting:** number of seeds, number of tasks, confidence intervals  

---

## Contributing
We welcome contributions.

### Add a new entry (short format)
Use this short template and keep each entry within a few lines:

```text
Name (Year, Venue):
Tags: [real/sim/synthetic/web] [tabletop/multi-scene] [short/long] [large-scale] [OOD] ...
Links: paper | website | code
