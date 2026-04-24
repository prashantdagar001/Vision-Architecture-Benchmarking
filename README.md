# Vision Architecture Benchmarking: U-Net vs. SegNet

This repository contains the full implementation and performance analysis of **U-Net** and **SegNet** architectures for semantic segmentation. This project was submitted as part of the requirements for the **Bachelor of Technology in Computer Science & Engineering** at **IIIT Sonepat**.

## 📌 Project Overview
The project explores pixel-wise classification to achieve detailed scene understanding. The primary focus is evaluating the trade-offs between segmentation accuracy and computational efficiency.

### Architectures Evaluated
* **U-Net:** A symmetric encoder-decoder model with skip connections that transfer feature maps to preserve fine-grained spatial details. Implemented with a **ResNet34** backbone.
* **SegNet:** An efficiency-focused architecture that reuses pooling indices from the encoder to guide upsampling, significantly reducing memory usage.

## 🛠️ Technology Stack
* **Frameworks:** TensorFlow, Keras
* **Libraries:** OpenCV (Image Processing), NumPy (Numerical Analysis), Matplotlib (Visualization)
* **Preprocessing:** Patchifying, normalization, and data augmentation

## 📊 Performance Comparison
| Metric | U-Net (ResNet34) | SegNet |
| :--- | :--- | :--- |
| **Dataset** | Semantic Drone Dataset | Oxford-IIIT Pet Dataset |
| **Accuracy** | **92.27%** | **87.15%** |
| **Complexity** | High (Detail Preservation) | Low (Resource Efficient) |

## 🚀 Key Insights
* **Detail Preservation:** U-Net is ideal for high-precision tasks like biomedical imaging where boundary accuracy is paramount.
* **Resource Optimization:** SegNet demonstrates competitive performance while being better suited for real-time applications such as autonomous driving.

## 👤 Author
* **Prashant Dagar**

## 📜 References
* Ronneberger et al. (2015), "U-Net: Convolutional Networks for Biomedical Image Segmentation".
* Badrinarayanan et al. (2017), "SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation".
