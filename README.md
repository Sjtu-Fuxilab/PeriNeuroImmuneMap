# PeriNeuroImmuneMap

**Multi-Scale Spatial Transcriptomics Framework for Perineural Neuroimmune Coupling**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)

---

## Overview

**PeriNeuroImmuneMap** is a research-grade computational pipeline for characterizing **perineural neuroimmune coupling**
using spatial transcriptomics and integrative downstream analyses.

The repository is organized as a **modular, notebook-first pipeline** with reproducible execution order, clear I/O conventions,
and publication-oriented outputs.

**Repository:** https://github.com/Sjtu-Fuxilab/PeriNeuroImmuneMap

---

## What this repository contains

- **01 — Data Processing & QC:** input harmonization, QC, preprocessing
- **02 — Nerve Injury Signature:** derivation, validation, benchmarking
- **03 — Immune Landscape:** spatial immune programs & external validation
- **04 — Communication Networks:** nerve–immune–tumor interactions (LR/network analysis)
- **05 — Circadian/Symptom Analysis:** cohort-scale analysis and translational stratification

---

## Repository structure

```text
PeriNeuroImmuneMap/
├── notebooks/
│   ├── 01_data_processing_qc.ipynb
│   ├── 02_nerve_signature_derivation.ipynb
│   ├── 03_immune_landscape_analysis.ipynb
│   ├── 04_communication_networks.ipynb
│   └── 05_circadian_symptom_analysis.ipynb
├── requirements.txt
├── environment.yml
├── LICENSE
└── README.md
```

> Note: Large datasets and generated outputs should not be committed. Keep the repo lean and reproducible via `.gitignore`.

---

## Installation

### Option A — Conda (recommended)

```bash
git clone https://github.com/Sjtu-Fuxilab/PeriNeuroImmuneMap.git
cd PeriNeuroImmuneMap

conda env create -f environment.yml
conda activate perineuroimmuemap
```

### Option B — Pip

```bash
pip install -r requirements.txt
```

---

## Usage

Launch Jupyter and run notebooks in order:

```bash
jupyter notebook
```

Execution order:

1. `notebooks/01_data_processing_qc.ipynb`
2. `notebooks/02_nerve_signature_derivation.ipynb`
3. `notebooks/03_immune_landscape_analysis.ipynb`
4. `notebooks/04_communication_networks.ipynb`
5. `notebooks/05_circadian_symptom_analysis.ipynb`

---

## Reproducibility expectations

- Deterministic seeds where applicable
- Explicit software versions (environment files)
- Separation of **data**, **code**, and **outputs**
- Notebook headers defining **Inputs / Outputs / Runtime**

---

## Citation

If you use this pipeline, please cite:

```bibtex
@article{zafar2026perineural,
  title     = {Perineural Neuroimmune Coupling Disrupts Circadian Regulation and Drives Behavioral Symptom Burden in Cancer},
  author    = {Zafar, Sanwal Ahmad and Qin, Wei and others},
  journal   = {Neuroimmunomodulation},
  year      = {2026},
  publisher = {Karger}
}
```

---

## Correspondence
Assoc. Prof. Wei Qin
Associate Dean, Institute of Industrial Engineering and Management 
Shanghai Jiao Tong University, China  
Email: wqin@sjtu.edu.cn
