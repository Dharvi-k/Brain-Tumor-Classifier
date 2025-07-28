# Brain-Tumor-Classifier
Brain tumor classification using MRI scans with deep learning and PyTorch.

# Brain Tumor Classification (ResNet18 + PyTorch)

Classifies brain MRI images into **4 categories**:
- **Glioma Tumor**
- **Meningioma Tumor**
- **Pituitary Tumor**
- **No Tumor**

---

## 📁 Datasets Used

1. **Main Dataset**:  
🔗 https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset
(Folders: `Training/`, `Testing/`)

2. **Additional Dataset**:  
🔗 https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri
(Used to boost training samples)

---

## 🏗️ Model Overview

- **Base Model**: ResNet-18 (pretrained)
- **Modified**: Final layer → 4 output classes
- **Accuracy**: ~91–92%
- **Loss**: CrossEntropyLoss  
- **Optimizer**: Adam  
- **Input Size**: 224×224  
- **Normalization**: ImageNet stats

---

## 📊 Evaluation & UI

- **Confusion Matrix** for performance
- **Sample MRI Visualizations**
- **Gradio Interface** for real-time image upload & prediction

---

## 💾 Model Weights

Trained model saved as: `brain_tumor_model_1.pth`  
✔️ You can load it directly for inference

---
## 🚀 How to Use

Simply open the notebook in Google Colab and run all cells.

> For real-time prediction, ensure that `gradio` is installed:
```python
!pip install gradio

