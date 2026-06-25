# Project and Fuse: A powerful Kernel independence test in high dimensions

## Introduction

This repository contains the code and data necessary to reproduce the numerical results reported in the main paper (**Sections 1** and **5**) and the supplementary material (**Section F**).



---

## Repository Structure


### Simulations (`simulations/`)

This folder contains the code for implementing the simulation studies in **Sections 1** and **5** of the main paper and **Section F** of the supplementary material, as well as the reproducible results. 

#### Subfolders
- `Method_code/`  
  Contains the code of the method proposed in the paper.

- `Simulation_code1/`  
  Contains the code and reproducible results for implementing experiments in **Sections 1 (main paper)** and **5**.

- `Simulation_code2/`  
  Contains the code and reproducible results for implementing experiments in **Section F (supplementary material)**.

## Codes

This section lists the Python scripts used to reproduce the numerical and empirical results in the paper.

| Script | Section / Context | Reproduces |
|--------|------------------|-------------|
| `PIKE.ipynb` | - | Core implementation; called by `ex1.ipynb`–`ex5.ipynb`, `pics1.ipynb`, `picsr.ipynb`, and `pic1.ipynb`. |
| `Ind.ipynb` | Section 5 & Supplementary | All baseline methods used in comparisons (dCor, HSIC, etc.). |
| `ex1.ipynb` – `ex5.ipynb` | Section 5 | All simulation results in Section 5 (Figures and Tables comparing PIKE with existing methods). |
| `pic1.ipynb` | Introduction | Example illustrating the power loss of classical kernel‑based tests in high dimensions (Figure 1, if applicable). |
| `pics1.ipynb` | Supplementary Material | Code for the non‑sparse dependence structure (Figure S1.). |
| `picsr.ipynb` | Supplementary Material | Sensitivity analysis with respect to the weight parameter \(r\) (Figure S2.). |
| `picsratio.ipynb` | Supplementary Material | Sensitivity analysis with respect to the sample partitioning ratio \(t\) (Figure S3.). |

## Requirements

All scripts are written in Python 3. Required packages include (but are not limited to):

- `numpy`, `scipy`
- `scikit-learn`,`torch`
- `dcor`,`jobib`,`hyppo`



