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

Here is how the three architectures stack up against each other on the dataset after final fine-tuning:

| Model Architecture | Accuracy | Precision | Recall / Sensitivity | F1-Score | Approx. Size | Training Profile |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **MobileNetV2** *(Baseline)* | ~93.80% | — | — | — | ~14 MB | Fast & Lightweight |
| **ResNet50** | 96.53% | 95.60% | **98.06%** | 96.82% | ~98 MB | Moderate |
| **EfficientNetV2-B0** | **98.61%** | **100.00%** | 97.42% | **98.69%** | ~29 MB | Fast & Optimized |

---

## 🔍 Key Takeaways

* **EfficientNetV2-B0 is the Overall Winner:** It achieved the highest accuracy (**98.61%**) and a perfect **100.00% Precision** (zero false positives!). It manages this while being roughly $3\times$ smaller in file size than ResNet50.
* **ResNet50 for Maximum Safety:** If the priority is to miss as few true positive cases as possible, ResNet50 yields the highest **Recall (98.06%)**, making it excellent at catching almost every actual target instance.
* **Architecture Matters:** Transitioning from the lightweight MobileNetV2 baseline to EfficientNetV2 provided a massive **+4.81%** net increase in validation accuracy. 

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


