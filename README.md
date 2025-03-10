# TumorScan.ai - Brain Tumor Detection System

![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange)
![Flask](https://img.shields.io/badge/Flask-2.0%2B-lightgrey)

TumorScan.ai is a web-based application that uses deep learning to detect brain tumors in MRI images. This application helps in early detection of brain tumors, potentially saving lives through timely diagnosis.

## Features

- Web-based interface for easy upload of MRI images
- Deep learning-powered tumor detection
- Instant results with medical recommendations
- Support for common image formats (JPG, JPEG, PNG)
- Responsive and user-friendly design

## Technologies Used

- Python 3.7+
- TensorFlow/Keras
- Flask (Web Framework)
- OpenCV (Image processing)
- Pillow (Image handling)
- NumPy

## Installation

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Steps

  1. Clone the repository:
  ```bash
  git clone https://github.com/Piyush79432/BrainTumor.git
  cd tumorscan.ai
  ```
  2. Install Dependencies:
  ```bash
  pip install -r requirements.txt
  ```
3. Download the pre-trained model file BrainTumor10Epochs.h5 and place it in the project root directory

### Usage
  1.Run the Flask application:
  ```bash
  python app.py
  ```
  2.Open your web browser and navigate to:
  ```bash
  http://localhost:5000
  ```
  3. Follow the on-screen instructions to upload an MRI image
  4.View the detection results:
     a.  "No Brain Tumor" - Negative result
     b. "Warning! Tumor detected..." - Positive result

### Project Structure
tumorscan.ai/
├── app.py                 # Main application file
├── BrainTumor10Epochs.h5  # Pretrained model (not included)
├── requirements.txt       # Dependency list
├── uploads/               # Uploaded images storage
├── templates/
│   ├── home.html          # Home page template
│   └── upload.html        # File upload template
└── static/                # Static files (CSS, JS, images)

###  Requirements
  Create a requirements.txt file with the following content:
  ```bash
  Flask==2.0.3
  tensorflow==2.15.0
  numpy==1.21.6
  Pillow==9.0.1
  opencv-python==4.5.5.64
  Werkzeug==2.0.3
  ```
  Save this as requirements.txt in your project root.

### Disclaimer
  This application is intended for research and educational purposes only. It should not be used as a substitute for professional medical diagnosis. Always consult a qualified healthcare provider for medical 
  concerns.

