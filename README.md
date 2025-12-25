# Semantic Segmentation with Fully Convolutional Networks (FCN-8s)

This repository contains an implementation and analysis of **semantic segmentation**
using **Fully Convolutional Networks (FCNs)**, following the seminal paper by
Long et al. (2015).

The project focuses on understanding how classification CNN architectures
can be transformed into dense, pixel-wise prediction models through
fully convolutional design and skip connections.

---

## Reference Paper
- Jonathan Long, Evan Shelhamer, Trevor Darrell  
  *Fully Convolutional Networks for Semantic Segmentation*  
  https://arxiv.org/abs/1411.4038

---

## Problem Setting
- Task: **Semantic Segmentation**
- Goal: Assign a semantic label to **every pixel** in an image
- Challenge:
  - Preserve fine spatial details
  - Combine high-level semantic information with low-level appearance cues

---

## Model Architecture
- **Fully Convolutional Network (FCN)**
  - Converted a classification CNN into a fully convolutional model
  - Replaced fully connected layers with convolution layers
- **FCN-8s architecture**
  - Combines predictions from:
    - Deep, coarse layers (semantic information)
    - Shallow, fine layers (spatial detail)
  - Uses skip connections and in-network upsampling
- Upsampling:
  - Learnable deconvolution layers for pixel-level prediction

---

## Key Takeaways
- Fully convolutional networks enable efficient, end-to-end semantic segmentation
- Skip connections are critical for recovering fine-grained spatial details
- Semantic segmentation requires balancing global context and local precision
