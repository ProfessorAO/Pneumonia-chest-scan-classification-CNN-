

# Pneumonia Chest Scan Classification CNN

## Overview
This repository contains a TensorFlow Convolutional Neural Network (CNN) model designed for the classification of chest scans, distinguishing between images with and without pneumonia. It offers both command-line argument passing and an interactive terminal menu, to train the AI on their own data, evaluate the model, and utilize additional features in a Jupyter Notebook environment.

## Features
- **Model Training**: Train the model on your dataset.
- **Model Evaluation**: Evaluate the model's performance on test data.
- **Image Prediction**: Use the model to predict individual images.
- **Data Handling**: Features for uploading files and mounting drives, beneficial for Jupyter Notebook users.
- **Versatility**: Compatible with different IDEs like VSCode or PyCharm through argument passing.

## Model Architecture
- Three convolutional layers.
- A flattened layer followed by a dense layer.
- Activation: ReLU is used in all layers except the final layer, which uses sigmoid for binary classification.

## Getting Started
### Configuration
1. Clone the repository to your local machine.
2. Ensure you have TensorFlow and other required libraries installed.

### Usage
Run the script with the required directories as arguments:

python script.py --train_dir <train_directory> --test_dir <test_directory> --val_dir <validation_directory>

Alternatively, use the interactive terminal menu by simply running the script without arguments:

python script.py

### Important Notes
- **Initial Configuration**: Configure the model first to initialize and train it. The model must be configured before evaluation or prediction.
- **Jupyter Notebook Users**: The mount drive and upload files feature is specifically designed for you. Other IDE users may ignore these features.
- **Data Directories**: Ensure the data directories are correctly set for training, testing, and validation.

## Contribution
Feel free to contribute to this project, whether it's by adding new features, improving the model, or fixing bugs, your input is welcome. 

## Results
loss: 0.1711 - accuracy: 0.9479
