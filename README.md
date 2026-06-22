# Modality Collapse Measurement Framework

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-ee4c2c.svg)](https://pytorch.org/)

**When do multimodal representations stop being modality-specific and become modality-invariant?**

This repository provides a framework for measuring and understanding **modality collapse** in multimodal medical imaging systems.

## Overview

Multimodal medical imaging models combine information from multiple modalities, such as FLAIR, T1, T1CE, and T2. As representations propagate through deep neural networks, modality-specific information may be preserved, gradually reduced, or become increasingly shared across modalities.

This framework provides a reproducible methodology for quantifying these representation dynamics across network depth.

## How is modality collapse measured?

**Modality Probe Classification**
Can the network still identify which modality a representation came from?

**Centered Kernel Alignment (CKA)**
How similar are representations across modalities?

**Participation Ratio (PR)**
Is the representation collapsing into a lower-dimensional subspace?

**Singular Vector Canonical Correlation Analysis (SVCCA)**
Do different modalities converge toward similar representational subspaces?

**Modality Ablation Studies**
How much does model performance depend on each modality?

## Features

* End-to-end multimodal representation analysis
* Layer-wise modality collapse measurement
* Statistical evaluation and uncertainty estimation
* Synthetic perturbation experiments
* Reproducible experimentation pipeline

## Repository Structure

```text
modality-collapse-framework/
├── README.md
├── LICENSE
├── requirements.txt
├── .gitignore
└── modality-collapse-measurement-framework.ipynb

```

## Contributing

Contributions, discussions, and suggestions are welcome. Please open an issue or submit a pull request.

For direct inquiries: **pronabpual77@gmail.com**


**Can we quantify how multimodal representations evolve from modality-specific to modality-invariant?**

This framework is designed to help answer that question.
