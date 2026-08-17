<div align="center">

# RMT-D

### A Random Matrix Theory-Based Denoising Method for Resting-State fMRI Data

**Xingkai Wen, Fusheng Guo, Yushi Wang, Feihong Liu, Shurong Zheng, Wen Wang**

<br>

![Method](https://img.shields.io/badge/Method-Random%20Matrix%20Theory-1f4e79?style=flat-square)
![Application](https://img.shields.io/badge/Application-rs--fMRI%20Denoising-2a7f9e?style=flat-square)
![Training](https://img.shields.io/badge/Training-Free-3b7a57?style=flat-square)
![Code](https://img.shields.io/badge/Code-Release%20upon%20acceptance-7f8c8d?style=flat-square)

</div>

---

## Overview

Unstructured random thermal noise can reduce the detection sensitivity of resting-state functional magnetic resonance imaging (rs-fMRI) and perturb blood oxygen level-dependent (BOLD) time series and functional connectivity (FC) estimates.

We propose **RMT-D**, a training-free and statistically interpretable denoising method based on random matrix theory (RMT).

For each target voxel, RMT-D constructs local Casorati matrices at multiple in-plane spatial scales and performs denoising through three main components:

1. **T--W-calibrated rank and noise-scale estimation**  
   A sequential test calibrated by the Tracy--Widom distribution jointly estimates the effective local rank and noise scale at each candidate spatial support.

2. **Voxel-wise spatial-support selection**  
   The spatial support is selected adaptively by balancing the fraction of explained spectral energy against relative rank complexity.

3. **Alignment-aware spectral shrinkage**  
   The latent singular-value amplitudes of the retained spectral components are estimated, and spectral shrinkage incorporates left- and right-singular-vector alignment coefficients to compensate for noise-induced singular-vector misalignment.

The final reconstruction retains only the denoised time series of the target voxel.

---

## Method Overview

The processing pipeline of RMT-D can be summarized as

```text
Observed rs-fMRI
      │
      ▼
Multiscale local Casorati matrices
      │
      ▼
Module A
T--W-calibrated joint estimation
of effective rank and noise scale
      │
      ▼
Module B
Voxel-wise spatial-support selection
      │
      ▼
Module C
Alignment-aware spectral shrinkage
and target-voxel reconstruction
      │
      ▼
Denoised rs-fMRI



