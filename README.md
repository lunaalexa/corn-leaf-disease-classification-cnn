Corn Leaf Disease Classification using CNN 🌽
Project Overview

This project was developed as part of my Deep Learning coursework to explore how Convolutional Neural Networks (CNNs) can be used to automatically classify corn leaf diseases.

Early disease detection plays an important role in preventing crop yield loss. However, manual diagnosis can be difficult because different diseases often exhibit similar visual symptoms. This project investigates how deep learning can assist in identifying diseases directly from leaf images.

The model classifies corn leaves into four categories:

Blight
Common Rust
Gray Leaf Spot
Healthy
Demo & Presentation
Project Explanation Video

[Insert Video Link Here]

This video explains:

Dataset exploration
Model architecture
Challenges encountered
Performance evaluation
Key findings and lessons learned
Dataset

The dataset consists of labeled corn leaf images belonging to four classes:

Class	Description
Blight	Corn leaf blight disease
Common Rust	Rust infection on corn leaves
Gray Leaf Spot	Gray leaf spot disease
Healthy	Healthy corn leaves

One challenge identified during exploration was class imbalance, particularly for the Gray Leaf Spot class, which contained significantly fewer samples than other classes.

Development Process
1. Dataset Exploration
Analyzed class distribution
Identified class imbalance issues
Investigated potential sources of misclassification
2. Baseline Model

Built an AlexNet-inspired CNN architecture as a baseline model.

This established a benchmark for evaluating future improvements.

3. Model Optimization

To improve performance and reduce overfitting, several architectural enhancements were introduced:

Batch Normalization
Global Average Pooling
Dropout Regularization

The goal was to improve generalization while preserving strong classification performance.

Challenges & Solutions
Challenge

Gray Leaf Spot was significantly harder to classify because:

It had fewer training samples
Its visual characteristics were often similar to Blight

This caused frequent confusion between the two classes during early experiments.

Solution

Rather than simply training longer, the model architecture was refined by incorporating:

Batch Normalization
Global Average Pooling
Dropout

These improvements helped the model learn more discriminative features and reduced overfitting.

Results
Key Outcomes
Achieved approximately 93% test accuracy
Reduced Gray Leaf Spot → Blight misclassification from 33% to 6.9%
Improved model stability and generalization performance
What I Learned

This project taught me that model evaluation goes far beyond accuracy scores.

By analyzing training and validation loss curves, I learned how to identify signs of overfitting and better understand whether a model was genuinely learning meaningful patterns.

This became one of the most valuable lessons I carried into future machine learning projects.

Tech Stack
Python
TensorFlow / Keras
NumPy
Scikit-learn
Matplotlib
Future Improvements

Potential next steps include:

Experimenting with transfer learning architectures such as ResNet or EfficientNet
Applying data augmentation techniques to further address class imbalance
Expanding the dataset with more Gray Leaf Spot samples
Deploying the model as a lightweight web application for real-time disease prediction
🌟 What Made This Project Special

This was the project that changed how I evaluate machine learning models.

Before this project, I focused heavily on accuracy metrics. Through discussions with my lecturer and repeated experimentation, I learned that loss curves often reveal insights that metrics alone cannot.

It was the first time I started paying close attention to whether a model was actually learning—or simply memorizing.
