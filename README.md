# Brain Tumor Segmentation Model Metrics

This repository contains comprehensive HTML reports for 5 brain tumor segmentation models trained on the BraTS2020 dataset.

## 📊 Model Performance Reports

### [Model Performance Dashboard](Model_Performance_Dashboard.html)
**Main entry point** - Interactive dashboard comparing all 5 models with detailed metrics and rankings.

### Individual Model Reports

1. **[HybridTransUNet++ V2](HybridTransUNet_V2_Validation_Metrics.html)** 🥇
   - **Best Overall Performance**
   - Dice Score: **75.56%** (Highest)
   - Recall: **83.58%** (Best for tumor detection)
   - Novel multi-component architecture combining RDB, ASPP, Dual Attention, TransUNet, and U-Net++

2. **[Swin-UNet](SwinUNet_Test_Metrics.html)** 🥈
   - Dice Score: 73.07%
   - Accuracy: 99.57% (Highest)
   - Swin Transformer-based architecture

3. **[TransUNet](TransUNet_Test_Metrics.html)** 🥉
   - Dice Score: 68.66%
   - Vision Transformer + U-Net hybrid

4. **[Attention U-Net](Attention_UNet_Test_Metrics.html)**
   - Dice Score: 62.28%
   - Precision: 88.79% (Highest)
   - U-Net with attention gates

5. **[Simple CNN](Simple_CNN_Test_Metrics.html)**
   - Dice Score: 60.57%
   - Fastest baseline model (~5M parameters)

## 🎯 Key Findings

- **🏆 Best for Tumor Detection**: HybridTransUNet++ V2 (83.58% recall - highest sensitivity)
- **🥇 Best Overall Performance (Dice)**: HybridTransUNet++ V2 (75.56%)
- **🎯 Highest Accuracy**: TransUNet (99.58%)
- **⚡ Best Precision (Lowest False Positives)**: Attention U-Net (88.79%)

## 📁 Dataset

- **Source**: BraTS2020 (Brain Tumor Segmentation Challenge 2020)
- **Training Patients**: 200 (Hybrid with K-fold), 60 test patients (other models)
- **Input**: Multi-modal MRI sequences (T2-weighted + FLAIR)
- **Task**: Binary segmentation (tumor vs non-tumor)

## 🔬 Evaluation Metrics

All reports include:
- Dice Coefficient (F1 Score)
- Intersection over Union (IoU)
- Accuracy, Precision, Recall
- Loss values
- Clinical interpretation
- Architecture details

## 🚀 Usage

Simply open `Model_Performance_Dashboard.html` in any web browser to explore all model comparisons and navigate to individual detailed reports.

---

**Project**: Brain Tumor Segmentation using Deep Learning  
**Date**: February 2026  
**Framework**: TensorFlow/Keras with mixed precision training
