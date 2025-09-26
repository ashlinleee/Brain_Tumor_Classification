# Brain Tumor Classification
This repository contains implementations of three deep learning models: ResNet, DenseNet and VGG16 for brain tumor classification using MRI images. The models classify MRI scans into four categories:  
**Meningioma  
No Tumor  
Glioma  
Pituitary Tumor**  
The goal of this project is to build and compare CNN models for accurate brain tumor detection and to analyze their performance across different architectures.

| Model        | Description                | Key Highlights                                                  |
| ------------ | -------------------------- | --------------------------------------------------------------- |
| **ResNet**   | Residual network based CNN | High F1 scores, very low false positives/negatives              |
| **DenseNet** | Densely connected CNN      | Highest overall accuracy (~97.5%), perfect "No Tumor" detection |
| **VGG16**    | Pretrained VGG16 based CNN | Fast convergence, high recall for gliomas, good for screening   |


**Results**
| Model    | Accuracy | Strength                                 | Weakness                                     |
| -------- | -------- | ---------------------------------------- | -------------------------------------------- |
| ResNet   | 94.8%    | Low FPR/FNR, high F1                     | Glioma detection weaker                      |
| DenseNet | 97.5%    | Perfect No Tumor detection, balanced     | Glioma recall slightly lower (~93.6%)        |
| VGG16    | 94%      | High recall for Glioma, fast convergence | Pituitary recall low (~84%), class confusion |

**Observation**  
**DenseNet** is the best performing model overall while VGG16 is very good for screening but requires fine-tuning for Pituitary detection.  
  
**References**
Kaggle Brain Tumor MRI Dataset
He, K., Zhang, X., Ren, S., & Sun, J. (2016). Deep Residual Learning for Image Recognition, CVPR.
Dorfner, F. J. (2025). A Review of Deep Learning for Brain Tumor Analysis in MRI, Nature Reviews Neurology.
Zahoor, M. M., et al. (2024). Brain Tumor MRI Classification Using a Novel Deep Convolutional Neural Network, Biomedicines, 12(7), 1395.
Simonyan, K., & Zisserman, A. (2015). Very Deep Convolutional Networks for Large-Scale Image Recognition, ICLR.
