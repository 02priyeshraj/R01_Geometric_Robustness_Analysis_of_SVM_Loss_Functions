# Datasets

This directory contains the datasets required to reproduce the experiments presented in the accompanying manuscript.

## Dataset Overview

The experiments use two categories of datasets:

1. **Synthetic datasets**
2. **Real-world benchmark datasets from the KEEL Repository**

---

## 1. Synthetic Datasets

The synthetic datasets are **not stored in this repository** because they are generated programmatically.

To reproduce the synthetic datasets, run the notebook:

```text
notebooks/Deviation_Synthetic_SVM.ipynb
```

The notebook automatically generates all synthetic datasets used in the experiments, including:

- Clean dataset
- Uniform label noise
- Gaussian label noise
- Feature noise
- Outlier datasets
- Combined noise scenarios

No additional downloads are required for the synthetic experiments.

---

## 2. KEEL Benchmark Datasets

The real-world experiments use benchmark datasets obtained from the **KEEL (Knowledge Extraction based on Evolutionary Learning) Repository**.

The following datasets are used:

- Heart Disease
- Pima Indians Diabetes
- Ionosphere
- Sonar (Mines vs. Rocks)

### Standard Datasets

Download the original benchmark datasets from:

https://sci2s.ugr.es/keel/category.php?cat=clas

### Attribute Noise Datasets

The experiments also use the KEEL attribute-noise versions (Noisy Train–Noisy Test protocol with 5% attribute noise).

These datasets can be downloaded from:

https://sci2s.ugr.es/keel/attributeNoise.php

### KEEL Repository

Official KEEL dataset repository:

https://sci2s.ugr.es/keel/datasets.php

---

## Directory Structure

After downloading the datasets, place them in this directory (or update the notebook paths accordingly).

Example:

```text
datasets/
│
├── Heart/
├── Pima/
├── Ionosphere/
└── Sonar/
```

The notebooks assume that the datasets are available locally before execution.

---

## Citation

If you use the KEEL datasets in your own research, please cite the original KEEL repository and the corresponding dataset publications as requested by the dataset providers.

---

## Notes

This repository distributes only the source code used for the experiments.

The KEEL datasets remain the property of their respective authors and are available from the official KEEL Repository.
