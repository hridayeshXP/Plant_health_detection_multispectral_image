 AI-Driven Smart Gardening: Plant Health Detection

This project implements a multimodal deep learning system for plant health detection using drone-based RGB images and spectral imaging data. The goal is to automatically classify plants as Healthy or Unhealthy and support precision agriculture for sustainable gardening.

Dataset
- **RGB Images:** 3024×4032 px per sample  
- **Spectral Data:** 18 bands, ranging from 410 nm to 940 nm  
- **Labels:** Binary (Healthy / Unhealthy)  
- **Mapping:** Each RGB image has a unique ID that corresponds to its spectral reading

-  Methodology

### Feature Extraction
- **Spectral Data Encoder**
  - Autoencoder (encoder-only)  
  - Compressed to **32-dimensional latent features**

- **Image Data Encoder**
  - Pretrained **ResNet-18 CNN**  
  - Extracted **512-dimensional image features**

- **Fusion Model**
  - Concatenated **32-dim spectral + 512-dim image features**  
  - Passed through fully connected layers for binary classification  

## Preprocessing
- **Image Augmentations:**
  - Resize, Normalization  
  - Random Flip, Rotation, Color Jitter  

- **Dataset Split:**
  - 60% Training, 40% Validation  

---

## Training
- **Optimizer:** Adam  
- **Loss Function:** Binary Cross Entropy Loss (BCELoss)  
- **Epochs:** 15  

## Results

- **Spectral Data Only:** ~98% Accuracy  
- **Image Data Only:** ~93% Accuracy  
- **Fusion Model:** Higher robustness and balanced performance

  
