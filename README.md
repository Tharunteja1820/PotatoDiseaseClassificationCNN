# Potato Disease Classification Using CNN

A deep learning project that uses Convolutional Neural Networks (CNN) with TensorFlow and Keras to classify potato leaf images into three categories: Early Blight, Late Blight, and Healthy.

## Project Overview

Plant diseases can significantly affect agricultural productivity. Early identification of diseases helps farmers take appropriate preventive measures.

This project implements a CNN-based image classification model to identify potato leaf diseases from images.

## Objectives

- Develop a CNN model for potato leaf disease classification.
- Perform image preprocessing and data augmentation.
- Train and evaluate the deep learning model.
- Classify potato leaves into three disease categories.

## Dataset

The project uses the **PlantVillage Dataset**, specifically the potato leaf images.

The model supports three classes:

1. Potato Early Blight
2. Potato Late Blight
3. Potato Healthy

**Dataset source:** [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)

Note: The dataset is not included in this repository because of its size. Download it separately and arrange the images according to the expected directory structure.

## CNN Architecture

The project uses a Convolutional Neural Network (CNN) for image classification.

### Workflow

```text
Input Potato Leaf Images
          |
          v
   Image Preprocessing
          |
          v
    Data Augmentation
          |
          v
    CNN Architecture
          |
          v
   Feature Extraction
          |
          v
   Classification Layer
          |
          v
    Model Prediction
          |
          v
   Three Output Classes
```

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Repository Structure

```text
PotatoDiseaseClassificationCNN/
|
|-- potato_disease_classification.ipynb
|
|-- models/
|   |-- 3.0/
|       |-- saved_model.pb
|       |-- keras_metadata.pb
|       |-- variables/
|
|-- requirements.txt
|-- README.md
|-- .gitignore
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/PotatoDiseaseClassificationCNN.git
cd PotatoDiseaseClassificationCNN
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Download the dataset

Download the PlantVillage dataset and arrange the potato images in the following structure:

```text
dataset/
    PlantVillage/
        Potato___Early_blight/
        Potato___Late_blight/
        Potato___healthy/
```

### 5. Run the notebook

Open Jupyter Notebook:

```bash
jupyter notebook
```

Run `potato_disease_classification.ipynb` to explore the preprocessing, model training, evaluation, and prediction workflow.

## Trained Model

The trained TensorFlow SavedModel is available in the `models/3.0/` directory.

It can be loaded using TensorFlow for inference.

## Future Improvements

- Develop a REST API using FastAPI.
- Build an interactive frontend using Streamlit.
