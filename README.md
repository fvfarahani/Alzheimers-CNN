# Building a CNN Model for Alzheimer's Diagnosis Using MRI

This project aims to train a convolutional neural network (CNN) classifier to predict whether an MRI scan of a patient shows signs of Alzheimer's disease or not. Transfer learning is used, specifically the ResNet50 pre-trained model as the base model, and custom layers are added on top to fine-tune the model for our specific task.

## Usage

**The `main.ipynb` file contains all the steps involved in the project.** The notebook is divided into different sections that correspond to the various steps of the project.

## Data Source

The Alzheimer's dataset used in this project can be downloaded from [Kaggle here](https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images). You will need to create an account on Kaggle to access the dataset.

## Project Steps

- Data Preparation
  - Setting up Directories and Classes
  - Data Augmentation (for Minor Label)
- TensorFlow (TF) Dataset Creation
- Building Model using Transfer Learning
  - Setting Callbacks
- Training and Validating the Model
- [Results](#results)
  - [Model Performance](#model-performance)
  - [Confusion Matrix](#confusion-matrix)
  - [Classification Report](#classification-report)
- Exporting Misclassified Images
- Exporting Model

## Results

<h3>Sample MRIs</h3>
<p align="center">
  <img src="https://github.com/fvfarahani/Alzheimers-CNN/blob/main/Figures/sample_MRIs.png?raw=true" alt="Sample MRIs" width="90%">
</p>

<h3>Model Performance</h3>
<p align="center">
  <img src="https://github.com/fvfarahani/Alzheimers-CNN/blob/main/Figures/model_performance.png?raw=true" alt="Model Performance" width="90%">
</p>

<h3>Confusion Matrix</h3>
<p align="center">
  <img src="https://github.com/fvfarahani/Alzheimers-CNN/blob/main/Figures/confusion_matrix.png?raw=true" alt="Confusion Matrix" width="55%">
</p>

<h3>Classification Report</h3>

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.81      | 0.96   | 0.88     | 640     |
| 1     | 0.68      | 0.26   | 0.37     | 191     |
|       |           |        |          |         |
| **Accuracy** |           |        | 0.80     | 831     |
| **Macro Avg** | 0.75      | 0.61   | 0.63     | 831     |
| **Weighted Avg** | 0.78   | 0.80   | 0.76     | 831     |
