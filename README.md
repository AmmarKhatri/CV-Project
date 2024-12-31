# Step-Wise Feasibility Study on Tumor Segmentation to Generative AI for Synthetic Brain MRI Data in Neuroimaging

This repository contains the workflow and code required for a step-wise feasibility study on tumor segmentation and its extension to generative AI for creating synthetic brain MRI data in neuroimaging. This document provides an overview of how to set up and run the experimentation.

---

## Overview

The project is divided into the following steps:  
1. **Tumor Segmentation**:  
   Training and evaluation of the segmentation model using SegResNet and the MONAI Decathalon Dataset.  
   - Dataset: [http://medicaldecathlon.com/]  
   - Kaggle example: [https://www.kaggle.com/code/raycarterrete/3d-monai-brain-segmentation]  

2. **Data Preparation**:  
   Extracting the largest cross-sections from the slices.  

3. **Generative AI for Synthetic Data**:  
   Generating synthetic MRI data with tumors using generative models like VAE and W-GANs.  
   - VAE: Trained on a larger dataset. Code available here:  
     [https://www.kaggle.com/code/raycarterrete/diffusion-vae-mri-data]  
   - GANs: Produced the best results.  
     - Trained on `generation_old.ipynb` and `generation.ipynb`.  
       - `generation_old.ipynb`: Used cross-section data with tumor brain scans.  
       - `generation.ipynb`: Trained on different datasets.

4. **Evaluation Metrics**:  
   Assessing the quality of segmentation and synthetic data.

---

## Training Time-lapse

1. GAN trained on a larger dataset (500 epochs):  
   Dataset: [https://www.kaggle.com/datasets/ashfakyeafi/brain-mri-images]  
   ![WGAN-GAN 128 Resolution](https://github.com/AmmarKhatri/CV-Project/blob/main/WGAN-GAN_128_Res_ins.gif)  

2. GAN trained on the Decathalon dataset:  
   Dataset: [http://medicaldecathlon.com/]  
   ![WGAN-GAN 256 Resolution](https://github.com/AmmarKhatri/CV-Project/blob/main/WGAN-GAN_256_Res_ins.gif)

---
