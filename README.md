# 🤟 Text-to-Sign Language Converter

A deep learning-based **Text-to-Sign Language Converter** that translates user-provided text into corresponding sign language gestures using **American Sign Language (ASL Digits)** and **Indian Sign Language (ISL)** datasets.

The project implements a complete machine learning pipeline including data preprocessing, CNN model training, evaluation, and real-time text-to-sign conversion.

---

## 📌 Project Overview

This project aims to bridge communication gaps by converting textual input into sign language representations.

The system uses two datasets:

- 🔢 **American Sign Language Digits Dataset** — for numerical digit recognition
- 🔤 **Indian Sign Language (ISL) Dataset** — for alphabet recognition

A Convolutional Neural Network (CNN) is trained to classify sign language images and generate corresponding sign outputs for user-entered text.

---

## ✨ Features

- ✅ Text-to-sign language conversion
- ✅ Supports digits and alphabetic characters
- ✅ CNN-based image classification
- ✅ Data augmentation for better generalization
- ✅ High model accuracy
- ✅ Confusion matrix & performance visualization
- ✅ Trained model saving/loading support
- ✅ End-to-end machine learning workflow

---

## 🛠️ Technologies Used

### Languages & Libraries
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- OpenCV
- Matplotlib
- Seaborn
- Scikit-learn

### Tools & Platforms
- Jupyter Notebook
- KaggleHub
- Google Colab / Jupyter

---

## 📂 Dataset Used

### 🔢 ASL Digits Dataset
Used for recognizing numerical hand gestures.

### 🔤 Indian Sign Language (ISL) Dataset
Used for recognizing alphabetic hand gestures.

Datasets are loaded using KaggleHub.

---

## ⚙️ Machine Learning Pipeline

### 1️⃣ Data Loading & Exploration
- Loaded datasets from KaggleHub
- Performed exploratory data analysis (EDA)
- Visualized label distributions

### 2️⃣ Data Preprocessing
- Resized images to **32×32**
- Converted images to RGB format
- Normalized pixel values
- Encoded labels numerically
- Applied categorical encoding

### 3️⃣ Train-Test Split
- Split datasets into training and testing sets
- Ensured balanced evaluation

### 4️⃣ CNN Model Architecture
The project uses a Sequential CNN model consisting of:

- Conv2D Layers
- BatchNormalization
- MaxPooling2D
- Dropout Layers
- Dense Layers

### 5️⃣ Data Augmentation
Implemented using `ImageDataGenerator`:
- Rotation
- Zoom
- Width/Height shifts

This improves model robustness and generalization.

### 6️⃣ Model Training
- Optimizer: **SGD**
- Loss Function: **categorical_crossentropy**
- Callback: **ReduceLROnPlateau**

### 7️⃣ Model Evaluation
Performance evaluated using:
- Accuracy plots
- Loss plots
- Confusion matrices

The trained models achieved high classification accuracy on both datasets.

### 8️⃣ Model Saving
Trained CNN models are saved for future inference and deployment.

---

## 🤖 Text-to-Sign Language Conversion

The final application allows users to input text, which is then:

1. Preprocessed
2. Mapped character-by-character
3. Converted into corresponding sign language images

This demonstrates the complete real-world implementation of the trained models.

---

## 📸 Output Preview

| Input Text | Sign Language Output |
|------------|----------------------|
| HELLO | Sequence of ISL signs |
| 123 | Sequence of ASL digit signs |

---

## 🚀 Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/text-to-sign-language-converter.git
