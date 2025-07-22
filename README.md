# BrainShield

**BrainShield** is a deep learning-based project for automated brain tumor classification using MRI images. It leverages Convolutional Neural Networks (CNNs) to distinguish between four types of brain conditions: glioma tumor, meningioma tumor, pituitary tumor, and no tumor.

## Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Approach](#approach)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Usage](#usage)
- [Requirements](#requirements)
- [How to Run](#how-to-run)
- [References](#references)

---

## Overview

BrainShield aims to assist medical professionals by providing a rapid, accurate, and automated diagnosis of brain tumors. The model is trained and validated on a publicly available MRI dataset and demonstrates promising results in multi-class classification.

## Dataset

- **Source:** [Kaggle - Brain Tumor Classification (MRI)](https://www.kaggle.com/datasets/navoneel/brain-tumor-classification-mri)
- **Classes:** 
  - Glioma Tumor
  - Meningioma Tumor
  - Pituitary Tumor
  - No Tumor
- **Structure:** Images are separated into `Training` and `Testing` folders, each containing subfolders for each class.

## Approach

- Images are loaded and resized to 150x150 pixels.
- Data is shuffled and split into train and test sets.
- Labels are one-hot encoded for multi-class classification.
- A deep CNN is implemented using Keras/TensorFlow.

## Model Architecture

The CNN model consists of:

- Multiple convolutional layers for feature extraction.
- MaxPooling layers to reduce spatial dimensions.
- Dropout layers to prevent overfitting.
- Dense layers for classification.

**Output:** Softmax layer for multi-class prediction.

## Results

- Training and validation accuracy and loss are plotted to monitor the learning process.
- The trained model can predict the class of unseen MRI images.

## Usage

1. **Clone the repository**
    ```bash
    git clone https://github.com/Jayalakshmi21/BrainShield.git
    cd BrainShield
    ```

2. **Install dependencies**
    ```bash
    pip install -r requirements.txt
    ```

3. **Download the dataset**
    - Download the dataset from [Kaggle](https://www.kaggle.com/datasets/navoneel/brain-tumor-classification-mri).
    - Place it under the appropriate directory, e.g., `/input/brain-tumor-classification-mri/`.

4. **Run the notebook**
    - Open `BrainSheild.ipynb` using Jupyter or Google Colab.
    - Execute each cell sequentially.

## Requirements

- Python 3.10+
- TensorFlow / Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Seaborn
- scikit-learn
- PIL (Pillow)
- ipywidgets

*(See `requirements.txt` for full details.)*

## How to Run

- Train the model using the provided notebook.
- Visualize performance using the included plots.
- Predict on new MRI images by passing them through the trained model.

## References

- [Brain Tumor Classification (MRI) Dataset](https://www.kaggle.com/datasets/navoneel/brain-tumor-classification-mri)
- [Keras Documentation](https://keras.io/)
- [TensorFlow Documentation](https://www.tensorflow.org/)

---

**Note:** This project is intended for research and educational purposes only. For clinical use, further validation is necessary.
