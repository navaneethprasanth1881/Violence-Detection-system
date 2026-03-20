# AI-Based Real-Time Violence Detection using MobileNetV2

## Overview
This project is an AI-powered surveillance system that detects violent activities in real-time using deep learning. It uses MobileNetV2 to classify video frames into violence and non-violence categories.

The system supports both live webcam input and recorded video files, making it useful for real-world surveillance applications.

## Features
- Real-time violence detection using webcam
- Supports video file input
- MobileNetV2-based deep learning model
- Data augmentation for improved accuracy
- Class balancing for better performance
- Confidence score display
- Prediction smoothing using frame averaging
- Automatic saving of detected violence frames

## Tech Stack
- Python
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib

## Project Structure
violence-detection/
│── dataset/
│── model/
│── saved_model/
│── violence_frames/
│── train.py
│── detect_webcam.py
│── detect_video.py
│── requirements.txt
│── README.md

## Installation
1. Clone the repository:
git clone https://github.com/your-username/violence-detection.git
cd violence-detection

2. Install dependencies:
pip install -r requirements.txt

## Usage
Train the model:
python train.py

Run real-time detection (webcam):
python detect_webcam.py

Run detection on video file:
python detect_video.py

## Model Details
- Architecture: MobileNetV2 (Transfer Learning)
- Input Size: 224 x 224
- Output: Binary Classification (Violence / Non-Violence)
- Loss Function: Binary Crossentropy
- Optimizer: Adam

## Performance
- Accuracy: ~91%
- Precision: ~92%
- Recall: ~91%
- Validation Accuracy: ~90%

(Note: Performance may vary depending on dataset and training conditions)

## Limitations
- Depends on dataset quality and diversity
- May not perform well in low-light or crowded scenes
- Limited to binary classification

## Future Improvements
- Multi-class activity detection
- Integration with alert systems
- Deployment on edge devices
- Improved accuracy with larger datasets

## Output
The system displays:
- Predicted label (Violence / Non-Violence)
- Confidence score
- Visual indicator bar
- Saves frames when violence is detected

## License
This project is open-source and available under the MIT License.
