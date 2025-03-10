# TumorScan.ai

TumorScan.ai is a Python application for brain tumor detection using deep learning. This project leverages a Convolutional Neural Network (CNN) built with TensorFlow and Keras, and provides a Flask-based web interface that allows users to upload brain scan images and receive immediate diagnostic predictions.

## Features

- **Brain Tumor Detection:** Classifies brain scan images as either "No Brain Tumor" or "Tumor Detected".
- **Training Pipeline:** Train a CNN model using your own dataset with images organized in `datasets/no/` and `datasets/yes/`.
- **Testing Script:** Evaluate individual images using a standalone testing script.
- **Evaluation & Results:** Generate ROC curves and other evaluation metrics with the provided analysis script.
- **Web Application:** User-friendly interface built with Flask for real-time image analysis.

## Project Structure

TumorScan.ai/ ├── app.py # Flask web application for real-time tumor detection ├── mainTest.py # Script to test the trained model on single images ├── mainTrain.py # Script to train the CNN model on brain scan datasets ├── results.py # Script for model evaluation and ROC curve plotting ├── datasets/ # Directory containing brain scan images │ ├── no/ # Images with no brain tumor │ └── yes/ # Images with brain tumor ├── uploads/ # Directory for storing user-uploaded images └── templates/ # HTML templates for the web application


## Installation

### Prerequisites

- Python 3.6 or higher
- pip package manager

### Dependencies

Install the required packages using pip:

# TumorScan.ai

TumorScan.ai is a Python application for brain tumor detection using deep learning. This project leverages a Convolutional Neural Network (CNN) built with TensorFlow and Keras, and provides a Flask-based web interface that allows users to upload brain scan images and receive immediate diagnostic predictions.

## Usage

### 1. Prepare Your Dataset
Place your brain scan images into the `datasets/` folder with the following structure:
- `datasets/no/` – images with no tumor
- `datasets/yes/` – images with a tumor

### 2. Run using Flsk
Run the training script to build and save your model:
```bash
python app.py

