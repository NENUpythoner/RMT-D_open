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

## Overview

Unstructured random thermal noise can reduce the detection sensitivity of resting-state functional magnetic resonance imaging (rs-fMRI) and perturb blood oxygen level-dependent (BOLD) time series and functional connectivity (FC) estimates. To address this issue, we propose RMT-D, a training-free denoising method based on random matrix theory (RMT). RMT-D constructs local Casorati matrices at multiple in-plane patch scales and selects the spatial support voxel by voxel by balancing spectral energy against relative rank complexity. At each candidate scale, a sequential test calibrated by the Tracy--Widom distribution jointly estimates the local signal rank and noise scale. RMT-D then applies spectral shrinkage that accounts for singular-vector misalignment to reconstruct the denoised signal. We evaluated RMT-D using simulated data with spatially varying Gaussian and Rician noise, acquired human rs-fMRI data, and controlled head-motion simulations. Among the compared methods, RMT-D achieved the lowest MSE and the highest PSNR across all tested noise types and levels. It also achieved the lowest FC errors at low-to-moderate noise levels while remaining competitive at the highest noise level. The simulated residuals more closely matched the known-noise reference in their spatial distribution. Exploratory analyses of the acquired human data showed that the RMT-D residuals contained less visually apparent anatomical structure. The controlled head-motion experiments further showed that applying RMT-D after motion correction generally yielded better denoising performance than applying the procedures in the reverse order. Overall, RMT-D provides a statistically interpretable approach for suppressing random thermal noise in rs-fMRI.

## Repository Contents

- High-resolution figures from the manuscript are available in this repository.
- The implementation code and demo examples of RMT-D will be released upon acceptance of the manuscript.

## Citation

Citation information will be updated after publication.
