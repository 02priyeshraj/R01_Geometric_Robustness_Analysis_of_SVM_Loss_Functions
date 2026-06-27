# Geometric Robustness Analysis of SVM Loss Functions with Linear Kernels Using Angular Deviation

> **Status:** 🟡 Manuscript Under Review

---

## Overview

This repository contains the complete implementation accompanying the research manuscript:

> **Geometric Robustness Analysis of SVM Loss Functions with Linear Kernels Using Angular Deviation**

The project presents a geometry-driven framework for evaluating the robustness of linear Support Vector Machines (SVMs) under different types of data perturbations. Rather than relying solely on classification accuracy, robustness is quantified using **angular deviation**, a geometric measure that captures the rotation of the decision boundary caused by noise and outliers.

The implementation includes comparative experiments involving three margin-based SVM loss functions—**Hinge Loss**, **Pinball Loss**, and **Eagle Loss**—along with **Extreme Learning Machine (ELM)** as a non-margin-based baseline. Experiments are conducted on both synthetically generated datasets and benchmark datasets from the KEEL Repository under controlled noise settings.

---

# Repository Structure

```text
.
├── datasets/
│   ├── README.md
│   └── (Download KEEL datasets here)
│
├── figures/
│
├── notebooks/
│   ├── Deviation_KEEL_SVM.ipynb
│   ├── Deviation_Synthetic_SVM.ipynb
│   ├── ELM.ipynb
│   ├── Hypothesis_testing.ipynb
│   └── Loss_functions_plot.ipynb
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

# Features

- Geometry-driven robustness analysis using angular deviation.
- Comparative implementation of Hinge, Pinball, and Eagle loss SVMs.
- Extreme Learning Machine (ELM) baseline implementation.
- Synthetic dataset generation under multiple controlled noise conditions.
- Robustness evaluation on KEEL benchmark datasets.
- Hyperparameter analysis using heatmaps.
- Statistical significance analysis using paired t-tests and Wilcoxon signed-rank tests.
- Publication-quality visualizations for all experimental results.

---

# Experimental Workflow

The repository reproduces the complete experimental pipeline described in the manuscript.

1. Visualize the SVM loss functions.
2. Generate synthetic datasets with controlled perturbations.
3. Train and evaluate SVM variants under different noise scenarios.
4. Train and evaluate the ELM baseline.
5. Perform robustness analysis on KEEL benchmark datasets.
6. Compute angular deviation for each experiment.
7. Conduct statistical hypothesis testing.
8. Generate figures and summary tables.

---

# Notebooks

## 1. Loss_functions_plot.ipynb

Generates the plots of the Hinge, Pinball, and Eagle loss functions used throughout the manuscript.

---

## 2. Deviation_Synthetic_SVM.ipynb

Generates synthetic datasets and evaluates robustness under controlled perturbations.

The notebook includes experiments with:

- Clean datasets
- Uniform label noise
- Gaussian label noise
- Feature noise
- Outliers
- Combined noise and outlier scenarios

---

## 3. Deviation_KEEL_SVM.ipynb

Performs robustness analysis on benchmark datasets obtained from the KEEL Repository.

Experiments include:

- Standard datasets
- Attribute-noise datasets
- Angular deviation computation
- Hyperparameter search
- Heatmap generation

---

## 4. ELM.ipynb

Implements the Extreme Learning Machine (ELM) baseline used for comparison with margin-based SVMs.

The notebook evaluates ELM under both synthetic and KEEL benchmark datasets using the same geometric robustness metric.

---

## 5. Hypothesis_testing.ipynb

Performs the statistical analysis reported in the manuscript.

Implemented statistical tests include:

- Paired t-test
- Wilcoxon signed-rank test

The notebook compares the robustness of Hinge, Pinball, Eagle, and ELM using angular deviation.

---

# Datasets

The experiments use two categories of datasets.

## Synthetic Datasets

Synthetic datasets are generated programmatically using

```text
notebooks/Deviation_Synthetic_SVM.ipynb
```

No external download is required.

---

## KEEL Benchmark Datasets

The real-world experiments use benchmark datasets from the KEEL Repository, including:

- Heart Disease
- Pima Indians Diabetes
- Ionosphere
- Sonar (Mines vs. Rocks)

Both standard datasets and attribute-noise variants are used.

Detailed download instructions are available in:

```text
datasets/README.md
```

---

# Installation

Clone the repository:

```bash
git clone https://github.com/02priyeshraj/R01_Geometric_Robustness_Analysis_of_SVM_Loss_Functions.git
```

Move into the repository:

```bash
cd R01_Geometric_Robustness_Analysis_of_SVM_Loss_Functions
```

Install the required packages:

```bash
pip install -r requirements.txt
```

---

# Running the Experiments

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Execute the notebooks in the following order:

1. `Loss_functions_plot.ipynb`
2. `Deviation_Synthetic_SVM.ipynb`
3. `Deviation_KEEL_SVM.ipynb`
4. `ELM.ipynb`
5. `Hypothesis_testing.ipynb`

---

# Software Requirements

The implementation is developed in Python.

Major dependencies include:

- NumPy
- Pandas
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- CVXOPT
- Tabulate
- Jupyter Notebook

Complete dependency information is provided in `requirements.txt`.

---

# Reproducibility

This repository is intended to facilitate the reproducibility of the experiments presented in the accompanying manuscript.

To reproduce the reported results:

1. Install all required dependencies.
2. Download the KEEL datasets as described in `datasets/README.md`.
3. Generate the synthetic datasets using `Deviation_Synthetic_SVM.ipynb`.
4. Execute the notebooks in the recommended order.

Where applicable, fixed random seeds are used to improve reproducibility.

---

# Publication Status

This repository accompanies the manuscript:

**Geometric Robustness Analysis of SVM Loss Functions with Linear Kernels Using Angular Deviation**

The manuscript is currently under peer review.

Publication details, DOI, and citation information will be added after acceptance.

---

# Authors

### Priyesh Raj

Department of Computer Science and Engineering

Maulana Azad National Institute of Technology (MANIT), Bhopal, India

Email: **[2211201347@stu.manit.ac.in](mailto:2211201347@stu.manit.ac.in)**

---

### Sanyam Shukla

Department of Computer Science and Engineering

Maulana Azad National Institute of Technology (MANIT), Bhopal, India

Email: **[sanyamshukla@manit.ac.in](mailto:sanyamshukla@manit.ac.in)**

---

# Citation

If you use this repository in your research, please cite the associated publication once it becomes publicly available.

Citation details will be updated after publication.

---

# License

This project is licensed under the MIT License.

See the `LICENSE` file for additional details.

---

# Acknowledgements

The real-world datasets used in this work were obtained from the KEEL Repository. We gratefully acknowledge the KEEL project and the original dataset contributors for making these benchmark datasets publicly available.

---

## Contact

For questions, suggestions, or issues regarding this repository, please open a GitHub Issue or contact the corresponding author via email.
