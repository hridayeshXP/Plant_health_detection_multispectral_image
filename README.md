# Multimodal UAV-Based AI Framework for Precision Plant Health Monitoring in Green Campuses

This repository contains the official implementation of the research work submitted to **The Visual Computer (Springer)** titled:

**Multimodal UAV-Based AI Framework for Precision Plant Health Monitoring in Green Campuses**

The work presents a UAV-driven multimodal deep learning framework that integrates multispectral reflectance data and RGB imagery for accurate plant health assessment in urban green environments.

---

## Abstract

Monitoring plant health in urban green spaces is essential for sustainable city development, yet conventional inspection methods remain labor-intensive and subjective. This work presents a multimodal UAV-based AI framework that integrates multispectral reflectance data with high-resolution RGB imagery for automated plant health monitoring. An 18-band multispectral sensor (410–940 nm) and RGB images captured using an unmanned aerial vehicle are used to collect complementary physiological and visual plant information. Spectral features are learned using an autoencoder-based encoder, while visual features are extracted using a pretrained ResNet-18 model. These representations are fused through a dual-branch neural network for binary plant health classification. Experiments conducted on data collected from the Green Nirma University Campus achieve a classification accuracy of 98.8%, demonstrating the effectiveness of multimodal data fusion for scalable and precise urban smart gardening applications.

---

## Methodology Overview

The proposed framework consists of three main components:

- **Multispectral Branch**  
  An autoencoder-based encoder is used to learn compact and discriminative representations from 18-band multispectral reflectance data.

- **RGB Image Branch**  
  A pretrained ResNet-18 model with frozen weights is employed to extract robust visual features from UAV-captured RGB images.

- **Multimodal Fusion Network**  
  Spectral and visual features are concatenated and passed through a fully connected fusion network to perform binary classification (Healthy / Unhealthy).



## Dataset Description

- **Sensor**: 18-band multispectral spectrometer (410–940 nm)  
- **Imaging**: High-resolution RGB images captured via UAV  
- **Environment**: Green Nirma University Campus  
- **Labels**: Binary (Healthy, Unhealthy)  
- Each RGB image is paired with its corresponding spectral record using a unique image identifier.

Dataset access:
- **Dataset link**: https://drive.google.com/drive/folders/193fcDUGWJRFBk7V7qC86p5gMPbxly09_?usp=drive_link
- **License**: Research and academic use only

---

## Experimental Results

- **Task**: Binary plant health classification  
- **Best Accuracy**: 98.8%  
- **Evaluation Metrics**:
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  
  - Matthews Correlation Coefficient (MCC)  
  - Balanced Accuracy  
  - Confusion Matrix  

The results demonstrate the advantage of multimodal fusion over unimodal approaches under real-world conditions.


