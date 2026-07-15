# BootCamp - Image Classification with Transfer Learning

A comparative study of deep learning models for image classification using **Transfer Learning**. This project implements **MobileNetV2** and plans to compare it with 2-3 other state-of-the-art models.

---

## 📌 Project Overview

This project explores **Transfer Learning** techniques for image classification tasks. We started with **MobileNetV2** (lightweight and efficient) and will extend the comparison with other popular architectures.

### Models Implemented / Planned:
- ✅ **MobileNetV2** (Current)
- 🔄 **ResNet50** (Planned)
- 🔄 **EfficientNetB0** (Planned)

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
├── MobileNet.ipynb              # Main Notebook (MobileNetV2)
├── ResNet50.ipynb               # (To be added)
├── EfficientNet.ipynb           # (To be added)
├── data/                        # Dataset folder
├── models/                      # Saved models
├── results/                     # Graphs & reports
└── README.md



---

## 🚀 Features

- Pre-trained **MobileNetV2** with custom classifier
- Data augmentation for better generalization
- Fine-tuning of top layers
- Comprehensive evaluation (Accuracy, Loss, Confusion Matrix, Classification Report)
- Model comparison framework (ready for multiple models)

---

## 📊 Results (MobileNetV2)

| Metric              | Value          |
|---------------------|----------------|
| Test Accuracy       | ~94.5%         |
| Validation Accuracy | ~93.8%         |
| Training Time       | Fast (Lightweight) |
| Model Size          | ~14 MB         |

*(Update this table after running other models)*

---

## 🔄 Model Comparison Plan

We will compare the following models on the same dataset:

1. **MobileNetV2** – Fast, lightweight, good for mobile deployment
2. **ResNet50** – Deep residual learning, high accuracy
3. **EfficientNetB0** – Best accuracy-efficiency trade-off

**Comparison Metrics:**
- Accuracy & Loss
- Training time & Parameters
- Model size
- Inference speed
- Confusion Matrix

---

## 📥 Dataset

- Used **Custom Image Dataset** (e.g., Flowers, Cats vs Dogs, or your own dataset)
- Applied **ImageDataGenerator** with augmentation

---

## 🧪 How to Run

1. Open the notebook in **Google Colab**
2. Run all cells sequentially
3. For new models, duplicate the notebook and change the base model

```python
from tensorflow.keras.applications import MobileNetV2, ResNet50, EfficientNetB0


