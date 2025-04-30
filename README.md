# Medical-Image-Processing-for-Brain-Tumor-Detection

A deep learning-powered system for accurate detection of brain tumors using medical image processing on MRI and CT scans. This project leverages Convolutional Neural Networks (CNNs) to assist in early diagnosis, potentially improving patient outcomes and saving lives.

---

## 📚 Introduction

Brain tumors are abnormal cell growths in the brain that can be benign or malignant. Early detection is crucial, yet often difficult due to subtle or overlooked symptoms like headaches. Traditional diagnosis requires expert radiological analysis, which can be time-consuming and subjective.

This project aims to build a reliable, automated deep learning model capable of detecting brain tumors from MRI and CT images with high precision, thus aiding medical professionals in early and accurate diagnosis.

---

## 🎯 Objectives

- Automate the detection of brain tumors using deep learning.
- Achieve high accuracy and reliability using CNN-based models.
- Evaluate performance on diverse medical imaging datasets (MRI, CT).
- Reduce diagnosis time and support healthcare decision-making.

---

## 🧠 Model Architecture

The model is a custom **Convolutional Neural Network (CNN)** designed for binary classification: tumor vs. no tumor.

### Architecture Summary:
- **Convolutional Layers**: Feature extraction (edges, textures, shapes).
- **ReLU Activation**: Non-linearity for complex feature learning.
- **MaxPooling Layers**: Spatial downsampling to reduce overfitting.
- **Dense Layers**: High-level feature interpretation.
- **Sigmoid Output**: Final probability of tumor presence.

> Loss Function: **Binary Cross-Entropy**  
> Optimizer: **Adam**  
> Evaluation Metrics: Accuracy, Precision, Recall, F1-Score

---

## 🏋️ Training Pipeline

1. **Data Preprocessing**  
   - Rescaling and normalization of images  
   - Data augmentation (rotation, zoom, flip)

2. **Dataset Splitting**  
   - Training set (~70%)  
   - Validation set (~15%)  
   - Test set (~15%)

3. **Model Training**  
   - Trained over multiple epochs with early stopping  
   - Monitored validation loss to prevent overfitting

4. **Performance Evaluation**  
   - Confusion matrix and classification report  
   - Accuracy ~95% on validation data

---

## 💼 Dataset

The model is trained on publicly available medical image datasets, including:

- MRI and CT scans of healthy and tumor-affected brains.
- Thousands of labeled images across diverse demographics.

> Datasets used: [Kaggle - Brain MRI Images](https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection)

---

## 🛠️ Technologies Used

- **Languages**: Python
- **Libraries**:
  - `TensorFlow`, `Keras` – Deep learning
  - `NumPy`, `Pandas` – Data handling
  - `Matplotlib`, `Seaborn` – Visualization
  - `OS`, `Math` – Utilities

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/brain-tumor-detector.git
cd brain-tumor-detector
