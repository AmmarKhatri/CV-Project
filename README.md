# Step-Wise Feasibility Study on Tumor Segmentation to Generative AI for Synthetic Brain MRI Data in Neuroimaging

This repository contains the workflow and code required for a step-wise feasibility study on tumor segmentation and its extension to generative AI for creating synthetic brain MRI data in neuroimaging. This document provides an overview of how to set up and run the experimentation.

---

## Overview

The project is divided into the following steps:  
1. **Tumor Segmentation**: Training and evaluation of segmentation model using SegResNet and MONAI Decathalon Dataset [http://medicaldecathlon.com/]
Check the following Kaggle link: Segmentation[https://www.kaggle.com/code/raycarterrete/3d-monai-brain-segmentation]
2. **Data Preparation**: We took out largest cross_sections from the slices.  
3. **Generative AI for Synthetic Data**: Generating synthetic MRI data with tumors using generative models like VAE and W-GANs
VAE was trained on a much larger dataset. Check code here[https://www.kaggle.com/code/raycarterrete/diffusion-vae-mri-data]
GANs produced the best results so we trained them on generation_old.ipynb and generation.ipynb files where cross-section data with tumor brain scans was used in old file while it was a different case for other file.
4. **Evaluation Metrics**: Assessing the quality of segmentation and synthetic data.


## Training time-lapse:
1. ![WGAN-GAN_128_Res_ins](https://github.com/AmmarKhatri/CV-Project/blob/main/WGAN-GAN_128_Res_ins.gif)
2. ![WGAN-GAN_256_Res_ins](https://github.com/AmmarKhatri/CV-Project/blob/main/WGAN-GAN_256_Res_ins.gif)
---
