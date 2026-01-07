#  Network Intrusion Detection System with Machine Learning

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Dataset](https://img.shields.io/badge/Dataset-NSL--KDD-orange.svg)](https://www.unb.ca/cic/datasets/nsl.html)

A Machine Learning-based Network Intrusion Detection System (NIDS) engineered to detect and classify malicious network activities using advanced ensemble methods like Random Forest and XGBoost.

---

##  Overview

This project implements an intelligent **Network Intrusion Detection System (NIDS)**. By analyzing traffic patterns from the **NSL-KDD** dataset, the system distinguishes between normal connections and various types of network attacks (DoS, Probe, R2L, U2R).

### Key Objectives
- **Automated Detection:** Identify network intrusions using supervised learning.
- **Model Comparison:** Evaluate and compare Random Forest and XGBoost algorithms.
- **Performance Optimization:** Minimize false positives for reliable security monitoring.

---

##  Features

- **Binary Classification:** Effective distinction between Normal traffic and Attacks.
- **Advanced Preprocessing:**
  - Label Encoding for categorical variables.
  - Standard Scaling for numerical consistency.
  - Handling of imbalanced data classes.
- **Model Suite:** Implementation of two powerful algorithms:
  1. **Random Forest**
  2. **XGBoost**
- **Evaluation:** Detailed Confusion Matrix and F1-Score analysis.
- **Visualization:** Comprehensive plots for feature importance and prediction distribution.

---

##  Dataset

**NSL-KDD Dataset**
Refined version of the classic KDD Cup 99 dataset, solving inherent redundancy issues.
- **Training Samples:** 125,973
- **Test Samples:** 22,544
- **Features:** 41 attributes (Duration, Protocol, Service, Bytes, Flags, etc.)

**Attack Types Covered:**
- **DoS** (Denial of Service)
- **Probe** (Surveillance and other probing)
- **R2L** (Unauthorized access from a remote machine)
- **U2R** (Unauthorized access to local superuser privileges)


##  Results

The model performance was evaluated using accuracy, precision, recall, and F1-score. **XGBoost** outperformed Random Forest, making it the selected model for this system.

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|:--------:|:---------:|:------:|:--------:|
| **Random Forest** | 77.13% | 76.5% | 78.2% | 77.3% |
| **XGBoost** | **81.00%** | **80.8%** | **82.1%** | **81.4%** |

### Key Findings
- **XGBoost** achieved the highest accuracy (**81%**), providing a better balance between detection rate and false alarms.
- The model effectively identifies **DoS** and **Probe** attacks.
- Feature selection significantly reduced training time without compromising accuracy.

---

##  Technologies Used
- **Python 3.8**
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn.
- **Environment:** Google Colab.
---
##  Authors
- **CHEBBOUT Rafik**

**Supervisor:** Mlle Y. YOUNSIOUI
**University:** Université Abderrahmane Mira de Béjaia (2025 - 2026)
