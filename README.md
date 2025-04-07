# Cattle Corral Optimization Algorithm (CCO)
## A Novel, Meta Heuristic, Nature Inspired, Feature Selection Algorithm

## Overview

Machine learning optimization often involves complex challenges like large search spaces and hyperparameter sensitivity, especially in domains like fake news detection. Nature-inspired metaheuristics (e.g., PSO, WOA) have emerged as powerful tools to address these issues.

This repository presents the **Cattle Corral Optimization (CCO)** algorithm, a novel metaheuristic building upon this field. CCO is inspired by the ecosystem around grazing cattle, translating animal behaviors into optimization strategies.

## How CCO Works

CCO uses a two-pronged search mechanism:

1.  **Egret-Inspired Global Search:** Mimics the strategic movement of egrets towards resource-rich areas (high-potential solutions).
2.  **Fly-Inspired Local Search:** Simulates the random, localized exploration of flies around cattle (refining known good solutions).

These behaviors are integrated within a population-based model designed for machine learning pipelines.

## Core Functionality & Features

*   **Hybrid Optimization:** Simultaneously optimizes model hyperparameters and selects informative feature subsets.
*   **Informed Initialization:** Uses pre-ranked features (weighted correlation & mutual information) to guide the initial search, improving convergence speed and solution quality.
*   **Efficiency:** Employs an early stopping mechanism based on fitness stagnation to avoid unnecessary computation.

## Repository Purpose

This repository provides the source code for the CCO algorithm, enabling its use and further development. 

**Key Contributions:**
*   Novel CCO Algorithm blending global (egret) and local (fly) search.
*   Hybrid feature selection and hyperparameter tuning framework.
*   Empirical validation demonstrating effectiveness.



### 📊 Feature Selection Results

| Metric      | None  | CCO   | HSDO  | WOA   | HHA   | GSF   | PSO   |
|-------------|-------|-------|-------|-------|-------|-------|-------|
| **AUC**     | 0.637 | 0.979 | 0.971 | 0.952 | 0.950 | 0.958 | 0.971 |
| **F1**      | 0.946 | 0.935 | 0.933 | 0.892 | 0.891 | 0.895 | 0.923 |
| **Accuracy**| 0.963 | 0.933 | 0.933 | 0.893 | 0.892 | 0.904 | 0.929 |
| **Precision**| 0.085 | 0.999 | 0.999 | 0.998 | 0.997 | 0.999 | 0.999 |
| **FPR**     | 0.001 | 0.001 | 0.001 | 0.002 | 0.002 | 0.002 | 0.001 |
| **FNR**     | 0.998 | 0.130 | 0.133 | 0.213 | 0.213 | 0.181 | 0.143 |
| **MCC**     | 0.008 | 0.879 | 0.874 | 0.804 | 0.803 | 0.822 | 0.867 |
| **n-feat**  | 21    | 9     | 9     | 15    | 12    | 10    | 10    |

**Legend:**
- **CCO**: Cattle Corral Optimization 
- **HSDO**: Hybrid Squirrel Dragonfly Optimization
- **WOA**: Whale Optimization Algorithm
- **HHA**: Horse Heard Optimization
- **GSF**: Grey Sail Fish Optimization
- **PSO**: Particle Swarm Optimization



### 🔗 Run on Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/INFO-3604-Project/Cattle-Corral-Project/blob/main/main.ipynb)

