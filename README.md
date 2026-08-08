<div align="center">

# RMT-D

### A Random Matrix Theory-Based Denoising Method for Resting-State fMRI Data

<br>

**Xingkai Wen · Fusheng Guo · Yushi Wang · Feihong Liu · Shurong Zheng · Wen Wang**

<br>

<img src="https://img.shields.io/badge/Application-rs--fMRI_Denoising-176B87?style=flat-square" />
<img src="https://img.shields.io/badge/Method-Random_Matrix_Theory-245B78?style=flat-square" />
<img src="https://img.shields.io/badge/Training-Training--Free-2E8B8B?style=flat-square" />
<img src="https://img.shields.io/badge/Code-Upon_Acceptance-B0B8C1?style=flat-square" />

<br><br>

> **A training-free random matrix theory framework for suppressing unstructured random thermal noise in resting-state functional MRI.**

</div>

---

## Overview

Unstructured random thermal noise can reduce the detection sensitivity of resting-state functional magnetic resonance imaging (rs-fMRI) and perturb blood oxygen level-dependent (BOLD) time series and functional connectivity (FC) estimates. To address this issue, we propose RMT-D, a training-free denoising method based on random matrix theory (RMT). RMT-D constructs local Casorati matrices at multiple in-plane patch scales and selects the spatial support voxel by voxel by balancing spectral energy against relative rank complexity. At each candidate scale, a sequential test calibrated by the Tracy--Widom distribution jointly estimates the local signal rank and noise scale. RMT-D then applies spectral shrinkage that accounts for singular-vector misalignment to reconstruct the denoised signal. We evaluated RMT-D using simulated data with spatially varying Gaussian and Rician noise, acquired human rs-fMRI data, and controlled head-motion simulations. Among the compared methods, RMT-D achieved the lowest MSE and the highest PSNR across all tested noise types and levels. It also achieved the lowest FC errors at low-to-moderate noise levels while remaining competitive at the highest noise level. The simulated residuals more closely matched the known-noise reference in their spatial distribution. Exploratory analyses of the acquired human data showed that the RMT-D residuals contained less visually apparent anatomical structure. The controlled head-motion experiments further showed that applying RMT-D after motion correction generally yielded better denoising performance than applying the procedures in the reverse order. Overall, RMT-D provides a statistically interpretable approach for suppressing random thermal noise in rs-fMRI.
---

## Figures

High-resolution figures from the manuscript are available in this repository.

<p align="center">
  <b>High-Resolution Manuscript Figures</b><br>
  <sub>Figures are provided for convenient visualization and reference.</sub>
</p>

---

## Code Release

The implementation code and demo examples of **RMT-D** will be released upon acceptance of the manuscript.

<div align="center">

![Code Status](https://img.shields.io/badge/RMT--D_Code-Coming_After_Acceptance-6C7A89?style=for-the-badge)

</div>

---

## Citation

Citation information will be updated after publication.

---

<div align="center">

<sub>
RMT-D · Random Matrix Theory · Resting-State fMRI · Training-Free Denoising
</sub>

</div>
