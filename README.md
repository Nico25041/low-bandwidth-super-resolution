# Performance Study of Upscaling Techniques for Massive Remote Sensing Data in Low Bandwidth Environments

This repository contains the research manuscript:

**"Performance Study of Upscaling Techniques for Massive Remote Sensing Data in Low Bandwidth Environments"**  
Authors: Escobedo, N., Phan, J., Zaluzec, K., & Korah, J.  
Institution: California State Polytechnic University, Pomona  

The work studies how different upscaling methods perform on Sentinel-2 remote sensing imagery when bandwidth and compute are constrained, comparing classical interpolation to deep super-resolution models.

This work was presented at **CSCSU 25**.

## Presentation

This work was presented at **CSCSU 25**.

- Event / program page (includes my name as presenter):  

https://cscsu-conference.github.io/index25.html


## Overview

Remote sensing platforms often cannot transmit or store full-resolution imagery due to **bandwidth limitations**. A common workaround is to send downsampled images and later **upscale** them closer to the user or at the edge.

This project evaluates:

- **Classical interpolation baselines**
  - Nearest neighbor  
  - Bilinear  
  - Bicubic  

- **Deep super-resolution models**
  - Laplacian Pyramid Super-Resolution Network (**LapSRN**)  
  - **LapSRN-Fusion**, a variant that leverages previously available high-resolution imagery from the same region

We analyze these methods under realistic constraints, focusing on:

- Reconstruction quality (e.g., MSE, PSNR, SSIM)  
- Runtime / computational cost on resource-limited devices  
- Trade-offs between visual quality and practicality for low-bandwidth, edge-focused pipelines  

## Relevance

While the experiments are grounded in **remote sensing and precision agriculture**, the underlying problem is broader:

- Upscaling images that were intentionally downsampled for **bandwidth** reasons  
- Performing reconstruction on **resource-constrained** devices  
- Balancing **quality of experience** vs. **bitrate** and **compute budget**

> Note: This is a project report / preprint version and may differ from any later published version.
> Copyright © 2024 Nicolas Escobedo. All rights reserved.
