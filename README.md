# Rock Paper Scissors Image Classification

## Overview
This project focuses on classifying hand gestures for the Rock-Paper-Scissors game using a Convolutional Neural Network (CNN) model. The dataset contains images of hand gestures (Rock, Paper, Scissors) captured on a green background. The analysis involves data preprocessing with augmentation, splitting the dataset into training and validation sets, and training a CNN model to classify the gestures. This project was developed as part of a submission for Dicoding by Richard Angelico Pudjohartono.

**Objectives**:
- Preprocess and augment the Rock-Paper-Scissors image dataset to improve model robustness.
- Split the dataset into training (60%) and validation (40%) sets for model evaluation.
- Develop and train a CNN model to classify hand gestures into three categories: Rock, Paper, and Scissors.
- Evaluate the model's performance to support applications like real-time gesture recognition in games or interactive systems.

## Dataset
The dataset used is the **Rock Paper Scissors Dataset** by Julien de la Bruère-Terreault (drgfreeman@tuta.io), licensed under CC-BY-SA 4.0. It was originally developed for a hobby project involving a Rock-Paper-Scissors game using computer vision and machine learning on the Raspberry Pi ([GitHub Repository](https://github.com/DrGFreeman/rps-cv)).

**Contents**:
- Total of 2,188 images:
  - `Rock`: 726 images
  - `Paper`: 710 images
  - `Scissors`: 752 images
- All images are RGB, 300x200 pixels, in `.png` format, taken on a green background with consistent lighting and white balance.
- Images are organized into three subfolders: `rock`, `paper`, and `scissors`.

**Data Issues**:
- The dataset is relatively balanced, but augmentation (rotation, zoom, flip, etc.) was applied to increase variability and prevent overfitting.
- No significant missing or corrupted data reported.

## Project Structure
The analysis is conducted in a Jupyter Notebook: `proyek_akhir.ipynb`. The notebook is structured as follows:
1. **Library Imports**: Imports libraries including TensorFlow, Keras, and ImageDataGenerator for image preprocessing.
2. **Data Loading**: Extracts and loads the Rock-Paper-Scissors dataset from a ZIP file.
3. **Data Preprocessing**: Applies augmentation and splits the dataset into training (1,314 images) and validation (874 images) sets.
4. **Model Building**: Constructs a CNN model with multiple convolutional and dense layers.
5. **Model Training**: Trains the model for 76 epochs and evaluates its performance.
6. **Visualization**: Plots training and validation accuracy/loss over epochs.

## Model Evaluation
The CNN model was evaluated using the following metrics:
- **Accuracy**: Measures the proportion of correctly classified images in the training and validation sets.
- **Loss**: Measures the categorical crossentropy loss during training and validation.

### Training & Validation Accuracy
[![Training Accuracy](https://github.com/angelalim88/RockPaperScissor-Image-Prediction/images/training_accuracy.png)]

## Evaluation Results
The training history reveals the following:
- **Accuracy**: The model achieved high accuracy on the training set (almost 100% in some epochs) and validation set (up to 100%), indicating strong performance.
- The model demonstrates reliable gesture classification, suitable for applications like real-time Rock-Paper-Scissors games.

## Paper Gesture Test
[![Paper Gesture Test](https://github.com/angelalim88/RockPaperScissor-Image-Prediction/images/test_model.png)]