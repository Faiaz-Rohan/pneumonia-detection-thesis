# Uncertainty-Aware U-Net Autoencoder for Pneumonia Detection in Chest X-Ray Images

Bachelor's Thesis — Department of Software Engineering, Daffodil International University
Supervisor: Most. Munira Tabassum, Lecturer

## Overview
An unsupervised deep learning framework (UA-UNetAE) that detects pneumonia in chest X-ray
images without requiring disease-labeled training data. The model learns the distribution of
normal anatomical structures and flags deviations as anomalies — a practical approach for
resource-limited clinical settings where labeled pathology data is scarce.

## Approach
- U-Net Autoencoder with symmetric skip connections to preserve anatomical detail during
  image reconstruction
- Monte Carlo Dropout for uncertainty estimation alongside reconstruction
- Hybrid anomaly score combining Mean Squared Error (MSE), Structural Similarity Index
  Measure (SSIM), and Gradient Error
- ROC-based threshold optimization for final classification

## Results (Kaggle Chest X-Ray Pneumonia dataset)
| Metric | Score |
|---|---|
| Accuracy | 80.30% |
| Precision | 91.74% |
| Recall | 66.60% |
| F1-score | 77.17% |
| ROC-AUC | 83.87% |

## Output
Generates uncertainty-guided anomaly heatmaps that visualize suspicious pulmonary regions,
supporting interpretable, annotation-efficient chest X-ray analysis.

## Files
- `thesis_paper.pdf` — full thesis document
- (add your code/notebooks here if you're including them)
