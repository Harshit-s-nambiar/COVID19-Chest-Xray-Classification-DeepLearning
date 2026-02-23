# COVID-19 Chest X-Ray Classification using Deep Learning

## 🔍 Project Summary

Developed a deep learning-based computer vision system to classify chest X-ray images into:

- COVID-19
- Normal
- Viral Pneumonia

Implemented transfer learning using pre-trained CNN architectures (VGG16 and ResNet50) to achieve high classification performance on a limited medical imaging dataset.

This project demonstrates practical skills in deep learning model development, transfer learning, image preprocessing, and model evaluation.

---

## 🧠 Technical Skills Demonstrated

- Deep Learning (CNN)
- Transfer Learning
- Computer Vision
- Medical Image Classification
- TensorFlow / Keras
- ResNet50 & VGG16
- Data Augmentation
- Model Evaluation & Optimization
- Performance Comparison
- Overfitting Analysis
- Scikit-learn Metrics

---

## 🏗 Model Architecture

### 1️⃣ VGG16 (Transfer Learning)
- ImageNet pre-trained weights
- Frozen convolutional base
- Custom Dense classifier head
- Softmax multi-class output

### 2️⃣ ResNet50 (Transfer Learning)
- ImageNet pre-trained weights
- Feature extraction approach
- GlobalAveragePooling layer
- Fully connected classifier

### 3️⃣ ResNet50 + Data Augmentation
- RandomFlip
- RandomRotation
- RandomZoom
- RandomContrast

---

## 📊 Model Performance Comparison

| Model | Train Accuracy | Validation Accuracy |
|-------|---------------|--------------------|
| VGG16 | 98% | 84.4% |
| ResNet50 | **99,6%** | **75.7%** |
| ResNet50 + Augmentation | 91.6% | 71.2% |

### ✅ Best Model: VGG16  
Achieved highest validation accuracy of **84.4%**.

---

## 📈 Key Learnings & Observations

- VGG16 outperformed ResNet50 due to residual connections enabling better feature learning.
- Slight overfitting observed due to small dataset size.
- Data augmentation did not significantly improve performance in this case.
- Validation accuracy aligned with manual accuracy_score verification after resolving dataset shuffling issues.

---

## 📁 Dataset

- Chest X-ray image dataset
- 3 Classes: COVID, Normal, Viral Pneumonia
- Directory-based structured dataset
- Preprocessed to 224x224 resolution

Dataset source: (https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset)

---

## ⚙️ Implementation Workflow

1. Load dataset using `image_dataset_from_directory`
2. Apply preprocessing and normalization
3. Use transfer learning (ImageNet weights)
4. Freeze base model layers
5. Add custom classification head
6. Compile using Adam optimizer
7. Train and validate model
8. Evaluate performance
9. Compare models in tabular format
10. Perform real image prediction

---

## 🛠 Tools & Libraries

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## 🎯 Practical Applications

- Automated medical image diagnosis
- AI-assisted radiology
- Healthcare AI systems
- Binary & multi-class image classification systems

---

## 👨‍💻 Author

Harshit S Nambiar
Aspiring Machine Learning Engineer  
