 HEAD
---
title: Emotion Recognition App
emoji: 😊
sdk: streamlit
sdk_version: "1.32.0"
app_file: implement.py
pinned: false
---

# Real-Time Emotion Recognition App

This application uses deep learning to perform real-time emotion recognition from webcam input. It can detect and classify seven different emotions: angry, fearful, happy, neutral, sad, and surprised.

## Features

- Real-time emotion detection using webcam
- Face detection using OpenCV's Haar Cascade
- Emotion classification using a trained deep learning model
- Live display of emotion probabilities
- User-friendly Streamlit interface

## Prerequisites

- Python 3.10 or higher
- Webcam
- Required Python packages (listed in requirements.txt)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/emotion-recognition-app.git
cd emotion-recognition-app
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Run the Streamlit app:
```bash
streamlit run implement.py
```

2. Open your web browser and navigate to the URL shown in the terminal (usually http://localhost:8501)

3. Click the "Start" button to begin emotion recognition
4. Click the "Stop" button to stop the webcam feed

## Project Structure

- `implement.py`: Main application file
- `t4.h5`: Trained emotion recognition model
- `haarcascade_frontalface_default.xml`: Face detection cascade file
- `requirements.txt`: Python package dependencies
- `packages.txt`: System dependencies

## Dependencies

### Python Packages
- streamlit==1.32.0
- opencv-python-headless==4.8.1.78
- numpy==1.24.3
- tensorflow==2.15.0
- protobuf==3.20.3
- h5py==3.10.0
- pillow==9.5.0


## How It Works

1. The application captures video from your webcam
2. OpenCV's Haar Cascade classifier detects faces in each frame
3. Detected faces are processed and fed into the emotion recognition model
4. The model predicts the emotion probabilities
5. Results are displayed in real-time with the highest probability emotion shown above the face

## Contributing

Feel free to submit issues and enhancement requests!

## Authors
- Aryan Thakur: https://github.com/Husky1024
- Aakanksha Malhotra: https://github.com/aakankshamalhotra
- Aastha Chaurasia: https://github.com/aastha2212

## License

This project is licensed under the MIT License - see the LICENSE file for details.

Hey there! Welcome to my Emotion Detector project, where I’ve combined deep learning magic with some cool tech to recognize human emotions. 
This project uses Python, Convolutional Neural Networks (CNNs), libraries (matplotlib etc, tensorflow, sklearn, keras etc), real-time face detection with OpenCV, and a sleek deployment on Streamlit to make emotion detection simple, interactive, and fun.

What Can This Do?
Detect emotions like happy, sad, angry, surprised, and more!
Works in real-time using your webcam. Lets you test on images and videos too.
Easy-to-use interface powered by Streamlit.

What’s Under the Hood?
Here’s what makes it all work:
CNNs: These neural networks are trained to recognize facial expressions and emotions.
OpenCV: Handles all the face detection and real-time image processing. 
Streamlit: Turns our project into a user-friendly web app.
Dataset: Trained using the Kaggle 2013 Emotion Dataset.

📂 How We Organized This emotion-detector/ 
├── data/ # Dataset goes here
├── models/ # Saved CNN models
├── app/ # Streamlit app files 
├── scripts/ # Python scripts for preprocessing and detection 
├── requirements.txt # List of required libraries 
├── README.md # You're reading it!
└── LICENSE # License information

Preprocessing: Faces are detected and cropped. Images are resized and normalized for better training. 
Training: We used a CNN trained on the Kaggle dataset to learn to identify emotions. 
Real-Time Detection: Your webcam captures your face. OpenCV detects your face and passes it to the model. The model predicts your emotion and displays it live! 
Deployment: The whole project is wrapped into a Streamlit app for easy access. 

🎯 Results Accuracy: Achieved a solid accuracy of 69% around on the test dataset.
Performance: Works smoothly in real-time with minimal lag.
63b424ea8df90d0c7419e699bf2d0b80cf2317dc
