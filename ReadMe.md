# Face Emotion Detection using CNNs

**Author:** Nikhil Yarra

## 🚀 Overview

This project implements a CNN-based image classification system to detect facial emotions (Happy or Sad) using deep learning. Multiple transfer learning models (VGG16, ResNet50, DenseNet121, MobileNetV2) were trained, evaluated, and compared on real-world facial image datasets.

## 📁 Dataset

* **Source:** Google Images (manually curated)
* **Classes:** HAPPY 😄 and SAD 😔
---

## 📊 Experimental Setup

* **Image Size:** 256x256
* **Batch Size:** 32
* **Epochs:** 50
* **Preprocessing:** Normalization, Cleaning, Data Augmentation
* **Models Used:**

  * VGG16
  * ResNet50
  * DenseNet121
  * MobileNetV2

---

## 🧠 Model Architecture (Example: VGG16-based)

* Feature extractor (frozen)
* Global Average Pooling
* Dense Layer (256 units, ReLU)
* Dropout (0.5)
* Output Layer (Sigmoid)

---

## 📈 Results Summary

| Model       | Accuracy   | Loss       |
| ----------- | ---------- | ---------- |
| VGG16       | **0.9785** | **0.1094** |
| DenseNet121 | 0.9604     | 0.1386     |
| ResNet50    | 0.8557     | 0.3540     |
| MobileNetV2 | 0.7474     | 0.5129     |

* **Best Model:** VGG16
* **Confusion Matrix:**
  ![VGG Confusion Matrix](insert-vgg-cm-image-link-if-hosted)

---

## 📌 Evaluation Metrics

* **Precision:** 0.5615
* **Recall:** 0.5638
* **F1-Score:** 0.5627
* **ROC AUC:** 0.5021
* **Classification Report:** Full details in the notebook output.

---

## 📊 Visualizations

* **Training vs Validation Accuracy (All Models)**
* **Confusion Matrices**
* **ROC Curve**
* **Precision-Recall Curve**
* **F1-Score vs Threshold**

---

## 🤖 Unseen Data Predictions

* Real-time prediction on unseen individual and batch images
* Folder-wise evaluation
* Final confusion matrix from 100 images (Happy vs Sad)

---

## 📚 References

1. [VGG](https://arxiv.org/abs/1409.1556)
2. [ResNet](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/He_Deep_Residual_Learning_CVPR_2016_paper.html)
3. [MobileNetV2](https://arxiv.org/abs/1801.04381)
4. [DenseNet](https://www.cv-foundation.org/openaccess/content_cvpr_2017/html/Huang_Densely_Connected_Convolutional_CVPR_2017_paper.html)

---

## 📌 Conclusion

This project confirms that transfer learning with CNNs like VGG16 can deliver high accuracy in emotion detection. It provides a strong foundation for scalable emotion-aware applications in healthcare, human-computer interaction, and sentiment analysis.

