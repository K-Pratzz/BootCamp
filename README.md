# BootCamp - Image Classification with Transfer Learning

A comparative study of deep learning models for image classification using **Transfer Learning**. This project implements **MobileNetV2** and plans to compare it with 2-3 other state-of-the-art models.

---

## 📌 Project Overview

This project explores **Transfer Learning** techniques for image classification tasks. We started with **MobileNetV2** (lightweight and efficient) and will extend the comparison with other popular architectures.

### Models Implemented:
- ✅ **MobileNetV2**
- 🔄 **ResNet50**
- 🔄 **EfficientNetB0**

---

## 🛠️ Technologies Used

- **TensorFlow / Keras**
- **Google Colab**
- **Transfer Learning** (pre-trained on ImageNet)
- **Data Augmentation**
- **Matplotlib & Seaborn** (Visualization)
- **Scikit-learn** (Metrics)

---

## 📁 Project Structure
BootCamp/
├── MobileNet.ipynb
├── ResNet50.ipynb
├── EfficientNet.ipynb
└── README.md



---

## 🚀 Features

- Pre-trained **MobileNetV2** with custom classifier
- Data augmentation for better generalization
- Fine-tuning of top layers
- Comprehensive evaluation (Accuracy, Loss, Confusion Matrix, Classification Report)
- Model comparison framework (ready for multiple models)

---
## 📊 Model Performance Comparison

Here is the breakdown of how the three configurations perform on the validation dataset:

| Model Architecture | Accuracy | Precision | Recall / Sensitivity | F1-Score | Approx. Size | Training Profile |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **MobileNetV2** | **98.96%** | 98.72% | **99.35%** | **99.04%** | ~14 MB | Fast & Lightweight |
| **EfficientNetV2-B0** | 98.61% | **100.00%** | 97.42% | 98.69% | ~29 MB | Fast & Optimized |
| **ResNet50** | 96.53% | 95.60% | 98.06% | 96.82% | ~98 MB | Moderate |

---

## 🔍 Key Takeaways

* **MobileNetV2 Dominates the Balance:** Surprisingly, the lightweight **MobileNetV2** baseline achieved the highest overall Accuracy (**98.96%**), Recall (**99.35%**), and F1-Score (**99.04%**). It represents the most efficient compromise between performance and deployment footprint (~14 MB).
* **EfficientNetV2-B0 for Zero Mistakes:** If your pipeline requires absolute certainty when predicting a positive case, **EfficientNetV2-B0** achieved a perfect **100.00% Precision**, meaning it returned zero false positives.
* **ResNet50 vs. Edge Backbones:** While **ResNet50** performs exceptionally well at **96.53%** accuracy, the parameter efficiency built into MobileNet and EfficientNet architectures proves superior for this specific image classification task.

**Comparison Metrics:**
- Accuracy & Loss
- Training time & Parameters
- Model size
- Inference speed
- Confusion Matrix

---

## 🧪 How to Run

1. Open the notebook in **Google Colab**
2. Run all cells sequentially
3. For new models, duplicate the notebook and change the base model

```python
from tensorflow.keras.applications import MobileNetV2, ResNet50, EfficientNetB0


