## Project Steps:
Data Preparation
Setting up Directories and Classes
Data Augmentation (for Minor Label)


# Building a CNN Model for Alzheimer's Diagnosis Using MRI

This project aims to train a convolutional neural network (CNN) classifier to predict whether an MRI scan of a patient shows signs of Alzheimer's disease or not. Transfer learning is used, specifically the ResNet50 pre-trained model as the base model, and custom layers are added on top to fine-tune the model for our specific task.

## Usage

**The `main.ipynb` file contains all the steps involved in the project.** The notebook is divided into different sections that correspond to the various steps of the project.

## Data Source

The Alzheimer's dataset used in this project can be downloaded from [Kaggle here](https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images). You will need to create an account on Kaggle to access the dataset.

## Project Steps

- [Usage](#usage)
- [Data Source](#data-source)
- [Project Structure](#project-structure)
- [Results](#results)
  - [Model Performance](#model-performance)
  - [Confusion Matrix](#confusion-matrix)

## Results

### Sample MRIs
![alt text](https://github.com/fvfarahani/Alzheimers-CNN/blob/main/Figures/sample_MRIs.png?raw=true)

### Model Performance
![alt text](https://github.com/fvfarahani/Alzheimers-CNN/blob/main/Figures/model_performance.png?raw=true)

<h3>Model Performance</h3>
<p align="center">
  <img src="https://github.com/fvfarahani/Alzheimers-CNN/blob/main/Figures/model_performance.png?raw=true" alt="Model Performance" width="50%">
</p>

<h3>Confusion Matrix</h3>
<p align="center">
  <img src="https://github.com/fvfarahani/Alzheimers-CNN/blob/main/Figures/confusion_matrix.png?raw=true" alt="Confusion Matrix" width="50%">
</p>

The confusion matrix for the model is shown below:

|                   | Predicted: Not Alzheimer's | Predicted: Alzheimer's |
|-------------------|----------------------------|------------------------|
| Actual: Not Alzheimer's | 55                         | 7                      |
| Actual: Alzheimer's     | 9                          | 52                     |


