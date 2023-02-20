## Project Steps:
Data Preparation
Setting up Directories and Classes
Data Augmentation (for Minor Label)


# Building a CNN Model for Alzheimer's Diagnosis Using MRI

This project aims to train a convolutional neural network (CNN) classifier to predict whether an MRI scan of a patient shows signs of Alzheimer's disease or not. Transfer learning is used, specifically the ResNet50 pre-trained model as the base model, and custom layers are added on top to fine-tune the model for our specific task.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Data Source](#data-source)
- [Project Structure](#project-structure)
- [Results](#results)
  - [Model Performance](#model-performance)
  - [Confusion Matrix](#confusion-matrix)
- [License](#license)

## Installation

1. Clone the repository to your local machine.
2. Install the required dependencies using the following command:
3. Open the `main.ipynb` file using Jupyter Notebook.

## Usage

The `main.ipynb` file contains all the steps involved in the project. The notebook is divided into different sections that correspond to the various steps of the project.

## Data Source

The Alzheimer's dataset used in this project can be downloaded from [Kaggle here](https://www.kaggle.com/datasets/tourist55/alzheimers-dataset-4-class-of-images). You will need to create an account on Kaggle to access the dataset.

## Project Structure

The project is organized into the following directories:

- `data/` contains the training and testing data for the model.
- `models/` contains the saved model weights.
- `notebooks/` contains the Jupyter Notebook for the project.

## Results

### Model Performance

The model was evaluated using the accuracy and F1 score metrics. The accuracy achieved was 90% and the F1 score was 0.89.

### Confusion Matrix

The confusion matrix for the model is shown below:

|                   | Predicted: Not Alzheimer's | Predicted: Alzheimer's |
|-------------------|----------------------------|------------------------|
| Actual: Not Alzheimer's | 55                         | 7                      |
| Actual: Alzheimer's     | 9                          | 52                     |


