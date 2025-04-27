# Real-time-Face-Detection

Real-Time Face Recognition using Eigenfaces and SVM
This project performs face recognition using PCA (Eigenfaces) and SVM classifier. It also includes real-time detection via webcam.

## Requirements
- Python 3.x
- pip (Python package installer)

## Install Required Libraries
pip install opencv-python numpy matplotlib scikit-learn gdown joblib

## How to Run
1. Download the code: save the handson2.py file to your working directory.
2. Run the Python script: python handson2.py
3. Program Flow:
- The script will automatically download the dataset (face_recognition.zip) from Google Drive and extract it.
- Preprocessing:
  a. Load all face images from the dataset.
  b. Detect faces using Haar Cascade Classifier.
  c. Crop, resize, and flatten the faces.
- Training:
  a. The data is split into training and testing sets.
  b. A pipeline consisting of Mean Centering, PCA, and SVM is trained.
- Evaluation:
  a. Prints a classification report.
  b. Plots the cumulative explained variance of PCA.
  c. Displays eigenfaces (PCA components).
- Model Saving: the trained model is saved as eigenface_pipeline.pkl.
- Real-time Recognition:
  a. Activates the webcam.
  b. Detects and recognizes faces in real-time.
  c. Displays the label and confidence score on the screen.
- Exit the Webcam: press q on your keyboard to quit the webcam display.

## Notes
- The dataset is automatically downloaded using gdown.
- Haar Cascade Classifier is used for face detection.
- PCA reduces the dimensionality of the face images.
- SVM is used for face classification.
- The model pipeline (eigenface_pipeline.pkl) can be reused for future inference.
- You need a working webcam for real-time face recognition.

