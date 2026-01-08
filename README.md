# VLA Datasets & Benchmarks (Vision-Language-Action)

A curated list of datasets and benchmarks for **Vision-Language-Action (VLA)** research.
This repository focuses on **data formats, evaluation protocols, and benchmark comparability**, with practical guidance on **which dataset/benchmark to use** for different research needs.

> Maintained by: *Your Name / Lab*  
> Scope: datasets + benchmarks + evaluation protocols (no model architecture deep dive)

---

## Table of Contents
- [How to Use This List](#how-to-use-this-list)
- [Taxonomy](#taxonomy)
- [Datasets](#datasets)
  - [Real-World Robot Datasets](#real-world-robot-datasets)
  - [Simulation and Synthetic Datasets](#simulation-and-synthetic-datasets)
  - [Multimodal / Tactile / Special Embodiments](#multimodal--tactile--special-embodiments)
- [Benchmarks](#benchmarks)
  - [Tabletop + Simple Tasks](#tabletop--simple-tasks)
  - [Tabletop + Long-Horizon / Complex Tasks](#tabletop--long-horizon--complex-tasks)
  - [Multi-Scene + Complex Tasks](#multi-scene--complex-tasks)
  - [Real-World Evaluation Suites](#real-world-evaluation-suites)
  - [Diagnostic Benchmarks](#diagnostic-benchmarks)
- [Evaluation Protocols & Metrics](#evaluation-protocols--metrics)
- [Contributing](#contributing)
- [Citation](#citation)

---

## How to Use This List
This repository is organized to answer three practical questions:

1. **What exists?**  
   What datasets and benchmarks are commonly used in VLA research?

2. **How are they used?**  
   What are the key data formats, action representations, task setups, and evaluation protocols?

3. **Which should I choose?**  
   Given a research goal (e.g., long-horizon tasks, object OOD, sim-to-real, multi-robot generalization), which datasets or benchmarks best match the need?

If you are new to VLA, start from:
- **[Taxonomy](#taxonomy)** for how we categorize datasets and benchmarks
- **[Evaluation Protocols & Metrics](#evaluation-protocols--metrics)** for comparability pitfalls

---

## Taxonomy
### Dataset dimensions
- **Source:** real robot, simulation, synthetic generation, web video
- **Embodiment:** single-arm, mobile manipulation, bimanual, multi-robot
- **Modalities:** RGB, RGB-D, proprioception, tactile, audio
- **Action representation:** delta-EEF, absolute-EEF, joint-delta, joint-velocity, skill tokens
- **Scale:** episodes / trajectories / robot hours

### Benchmark dimensions
- **Environment structure:** tabletop vs multi-scene
- **Task horizon:** short-horizon vs long-horizon
- **Generalization splits:** object OOD, scene OOD, task OOD, embodiment shift
- **Metrics:** success rate, progress score, efficiency, safety

---

# Datasets

## Real-World Robot Datasets
> Real robot demonstrations, typically expensive but high fidelity.

### **Dataset Name (Year)**
- **Tasks:** ...
- **Embodiment:** ...
- **Modalities:** ...
- **Actions:** ...
- **Scale:** ...
- **Highlights:** ...
- **Limitations:** ...
- Links: [[paper]]() [[website]]() [[code]]()

(Repeat)

---

## Simulation and Synthetic Datasets
> Simulation data and synthetic generation pipelines for scalability, often with sim-to-real gaps.

### **Dataset Name (Year)**
- **Tasks:** ...
- **Embodiment:** ...
- **Modalities:** ...
- **Actions:** ...
- **Scale:** ...
- **Highlights:** ...
- **Limitations:** ...
- Links: [[paper]]() [[website]]() [[code]]()

---

## Multimodal / Tactile / Special Embodiments
> Datasets involving tactile sensing, mobile manipulation, bimanual hands, or non-standard robots.

### **Dataset Name (Year)**
- **Tasks:** ...
- **Embodiment:** ...
- **Modalities:** ...
- **Actions:** ...
- **Scale:** ...
- **Highlights:** ...
- **Limitations:** ...
- Links: [[paper]]() [[website]]() [[code]]()

---

# Benchmarks

## Tabletop + Simple Tasks
> Typically short-horizon manipulation in tabletop scenes.

### **Benchmark Name (Year)**
- **Setup:** ...
- **Tasks:** ...
- **Observation/Action:** ...
- **Splits:** ...
- **Metrics:** ...
- **Protocol notes:** reset policy, human intervention, seeds, etc.
- **What it tests well:** ...
- **What it misses:** ...
- Links: [[paper]]() [[website]]() [[code]]()

---

## Tabletop + Long-Horizon / Complex Tasks
> Longer horizon tasks and instruction chaining, often to study compounding errors.

### **Benchmark Name (Year)**
- (same template)

---

## Multi-Scene + Complex Tasks
> Navigation + manipulation, multi-room scenes, compositional tasks.

### **Benchmark Name (Year)**
- (same template)

---

## Real-World Evaluation Suites
> Benchmarks that require physical robots or standardized real-world setups.

### **Benchmark Name (Year)**
- (same template)

---

## Diagnostic Benchmarks
> Benchmarks designed to isolate specific capabilities, such as grounding or physical reasoning.

### **Benchmark Name (Year)**
- (same template)

---

# Evaluation Protocols & Metrics
This section summarizes common sources of inconsistency that make benchmark results hard to compare:

- **Success criteria:** binary success vs graded progress
- **Reset policy:** scripted resets vs human resets vs autonomous resets
- **Generalization splits:** object OOD vs scene OOD vs task OOD (definitions vary)
- **Embodiment shift:** evaluation across robots with different DoF and action spaces
- **Safety metrics:** collisions, unsafe contact, drop rates
- **Reporting:** number of seeds, number of tasks, confidence intervals

We recommend including:
- explicit split definitions,
- standardized metrics and task seeds,
- and reporting variance across runs.

---

## Contributing
We welcome contributions.

### Add a new entry
Please follow the template below:

```text
Name (Year):
- Tasks:
- Embodiment:
- Modalities:
- Actions:
- Scale:
- Highlights:
- Limitations:
- Links: paper / website / code
