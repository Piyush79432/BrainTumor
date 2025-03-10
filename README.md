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

### 2. Train the Model
Run the training script to build and save your model:

```bash
python mainTrain.py
Retrain the model (if needed) and predict on the test set.
Plot and display the ROC curve.
Save the evaluated model as BrainTumorModel.h5.
### 4. Test the Model on a Single Image
To test the model on a specific image, run:

```bash
Copy
Edit
python mainTest.py
Make sure to update the image path in the script if needed.```

### 5. Run the Web Application
Launch the Flask web application with:

bash
Copy
Edit
python app.py
Then, open your browser and go to http://127.0.0.1:5000/ to use the upload interface for real-time predictions.

## Model Details
The CNN model architecture includes:

Multiple convolutional layers with ReLU activation and max pooling.
A dense (fully connected) layer with dropout for regularization.
A final dense layer with softmax activation for binary classification (tumor vs. no tumor).
Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your improvements or bug fixes. For major changes, please open an issue first to discuss what you would like to change.


## Acknowledgements
Built with TensorFlow, Keras, and Flask.
Thanks to the open-source community for the development tools and libraries that made this project possible.
