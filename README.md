# Corn Leaf Disease Classification using CNN 🌽

## Project Overview

This project was developed as part of my Deep Learning coursework to explore how Convolutional Neural Networks (CNNs) can be used to automatically classify corn leaf diseases.

Early disease detection is important for preventing crop yield loss, but manual diagnosis can be time-consuming and often requires agricultural expertise. This project investigates how deep learning can assist in identifying diseases directly from corn leaf images.

The model classifies corn leaves into four categories:

- Blight
- Common Rust
- Gray Leaf Spot
- Healthy

---

## 🎥 Project Explanation

### Video Presentation
Watch the Project Explanation : https://drive.google.com/drive/folders/12CHuPERJCBcxLI4NBCk5dda70K3Rzl-S

This video covers:

- Dataset exploration
- CNN architecture design
- Model improvements
- Performance evaluation

---

## 📊 Dataset

The dataset consists of labeled corn leaf images belonging to four classes:

| Class | Description |
|---------|-------------|
| Blight | Corn leaf blight disease |
| Common Rust | Rust infection on corn leaves |
| Gray Leaf Spot | Gray leaf spot disease |
| Healthy | Healthy corn leaves |

One challenge identified during exploration was class imbalance, particularly for the Gray Leaf Spot class, which contained significantly fewer samples than other classes.

---

## 🔍 Development Process

### 1. Dataset Exploration

- Analyzed class distribution
- Identified class imbalance issues
- Investigated sources of misclassification

### 2. Baseline Model

Built an AlexNet-inspired CNN architecture as a baseline model.

This established a benchmark for evaluating future improvements and understanding model limitations.

### 3. Model Optimization

To improve performance and reduce overfitting, several architectural enhancements were introduced:

- Batch Normalization
- Global Average Pooling
- Dropout Regularization

The goal was to improve feature extraction and generalization performance.

---

## ⚠️ Challenges & Solutions

### Challenge

Gray Leaf Spot was significantly harder to classify because:

- It had fewer training samples
- Its visual characteristics were often similar to Blight

As a result, the baseline model frequently confused these two classes.

### Solution

Rather than simply increasing training time, the model architecture was refined by incorporating:

- Batch Normalization
- Global Average Pooling
- Dropout

These improvements helped the model learn more discriminative features while reducing overfitting.

---

## 📈 Results

### Key Outcomes

- Achieved approximately **93% test accuracy**
- Reduced Gray Leaf Spot → Blight misclassification from **33% to 6.9%**
- Improved model stability and generalization performance

---

## 💡 Key Learnings

- Architectural improvements can have a greater impact than simply training a model longer.
- Class imbalance can significantly affect model performance and should be addressed early.
- Evaluating loss curves is just as important as monitoring accuracy metrics.

---

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- NumPy
- Scikit-learn
- Matplotlib

---

## 🚀 Future Improvements

Potential next steps include:

- Experimenting with transfer learning models such as ResNet or EfficientNet
- Applying advanced data augmentation techniques
- Expanding the dataset with more Gray Leaf Spot samples
- Deploying the model as a lightweight web application for real-time disease classification

---

## 🌟 What Made This Project Special

This was the project that changed how I evaluate machine learning models.

Before this project, I focused heavily on accuracy metrics. Through repeated experimentation and feedback from my lecturer, I learned that loss curves often reveal insights that metrics alone cannot.

It was the first time I started paying close attention to whether a model was actually learning—or simply memorizing.

---


## 👤 Author

**Luna Alexa**  
Data Science Student at BINUS University
---

**BINUS University — Deep Learning Project (2026)**
