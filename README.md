# Alzheimer's Disease Detection using CNNs

## Overview
This project focuses on detecting and classifying Alzheimer's disease severity using a Convolutional Neural Network (CNN). The model is trained on MRI brain scans from the OASIS dataset and classifies images into four categories:

- **Non-Demented**
- **Very Mild Demented**
- **Mild Demented**
- **Moderate Demented**

The goal is to improve classification accuracy and handle class imbalance while comparing **ordinal vs. categorical classification** techniques.

## Dataset
- **Source:** OASIS Dataset (Open Access Series of Imaging Studies)
- **Class Distribution:**
  - Non-Demented: **67,222 scans**
  - Very Mild Demented: **13,725 scans**
  - Mild Demented: **5,002 scans**
  - Moderate Demented: **488 scans**
- **Challenge:** Significant class imbalance requiring data augmentation and balancing techniques.

## Model Architecture
This project utilizes **CNN-based architectures** for classification:
- **Pre-trained Models:**
  - EfficientNetB0
  - EfficientNetV2B1
- **Layers:**
  - Convolutional layers for feature extraction
  - Batch Normalization & Dropout for regularization
  - Fully Connected Layers for classification

## Performance Metrics
- **Precision, Recall, F1-score**
- **ROC-AUC Score**
- **Confusion Matrix**
- **Class-wise evaluation to mitigate imbalance issues**

## Key Research Questions
1. Does **ordinal classification** (preserving order among classes) outperform **categorical classification**?
2. What impact does **handling class imbalance** have on model performance?
3. Which **pre-trained model** achieves better results?

## Installation & Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/alzheimer-detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd alzheimer-detection
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Jupyter Notebook:
   ```bash
   jupyter notebook final-dl-project-alzheimer-s-detection.ipynb
   ```

## Results & Findings
- The **ordinal classification approach** improved accuracy compared to categorical classification.
- **EfficientNetV2B1** outperformed EfficientNetB0 in terms of precision and recall.
- **Data augmentation** helped mitigate class imbalance, leading to better generalization.

## Future Improvements
- Experiment with additional **pre-trained models** (e.g., ResNet, DenseNet).
- Implement **attention mechanisms** to improve feature extraction.
- Deploy the model using **Flask or FastAPI** for real-world application.

## Author
Abishekdakshna R


