<div align="center">

# RMT-D

### A Random Matrix Theory-Based Denoising Method for Resting-State fMRI Data

**Xingkai Wen, Fusheng Guo, Yushi Wang, Feihong Liu, Shurong Zheng, Wen Wang**

<br>

![Method](https://img.shields.io/badge/Method-Random%20Matrix%20Theory-1f4e79?style=flat-square)
![Application](https://img.shields.io/badge/Application-rs--fMRI%20Denoising-2a7f9e?style=flat-square)
![Status](https://img.shields.io/badge/Code-Coming%20Soon-7f8c8d?style=flat-square)

</div>

---

## Abstract

Unstructured random thermal noise can reduce the detection sensitivity of resting-state functional magnetic resonance imaging (rs-fMRI) and perturb blood oxygen level-dependent (BOLD) time series and functional connectivity (FC) estimates. To address this issue, we propose RMT-D, a training-free denoising method based on random matrix theory (RMT). RMT-D constructs local Casorati matrices at multiple in-plane patch scales and selects the spatial support voxel by voxel by balancing spectral energy against relative rank complexity. At each candidate scale, a sequential test calibrated by the Tracy--Widom distribution jointly estimates the local signal rank and noise scale. RMT-D then applies spectral shrinkage that accounts for singular-vector misalignment to reconstruct the denoised signal. We evaluated RMT-D using simulated data with spatially varying Gaussian and Rician noise, acquired human rs-fMRI data, and controlled head-motion simulations. Among the compared methods, RMT-D achieved the lowest MSE and the highest PSNR across all tested noise types and levels. It also achieved the lowest FC errors at low-to-moderate noise levels while remaining competitive at the highest noise level. Overall, RMT-D provides a statistically interpretable approach for suppressing random thermal noise in rs-fMRI.

---

## Repository Contents

This repository archives research resources associated with the RMT-D study.

- **`Fig_1.pdf`**: High-resolution RMT-D framework figure.
- **`IV_Results_and_Discussion/`**: Figures and tables generated from the experimental analyses.
- **`Code/`**: Implementation resources for RMT-D and the experiments.

---

## Experimental Results

The experimental results are organized into four sections for convenient inspection:

- **A. Denoising Results on Simulated Data**  
  Gaussian- and Rician-noise simulation results and residual analyses.

- **B. Exploratory Residual Analysis of Acquired Human Data**  
  Residual analyses for acquired human rs-fMRI data.

- **C. Controlled Head-Motion Results**  
  Results under controlled head motion and different processing orders.

- **D. Ablation Study**  
  Results for different combinations of Modules A, B, and C.

The figures and tables in these folders are organized according to their corresponding experimental analyses.

---

## Availability

High-resolution figures and organized experimental results are currently archived in this repository.

The simulated dataset, the complete implementation of RMT-D, the accompanying code for all experiments, and demonstration examples will be publicly released upon acceptance of the manuscript.

---

## Citation

Citation information will be updated after publication.
