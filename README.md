GISLR_sign-language: Real-Time ASL Recognition with Transformer Model

This repository contains a transformer-based model for real-time American Sign Language (ASL) recognition. The model leverages a state-of-the-art transformer architecture to interpret ASL gestures from live video input and integrates the Gemini API to construct coherent English sentences from recognized signs. This project aims to enhance communication accessibility for ASL users.

Project Overview

The GISLR_sign-language project provides a robust solution for real-time ASL recognition. It captures live video using OpenCV, processes gestures with MediaPipe’s holistic tracking, predicts signs using a TensorFlow Lite transformer model, and generates meaningful sentences via the Gemini API. The system is designed for seamless, on-the-fly translation of ASL gestures into text, making it a valuable tool for communication.

Features





Real-Time ASL Recognition: Detects and recognizes ASL gestures in real-time from video input.



Transformer Architecture: Utilizes a lightweight TensorFlow Lite transformer model for high-accuracy sign prediction.



Sentence Construction: Integrates the Gemini API to form grammatically correct English sentences from recognized ASL words.



Live Video Input: Supports webcam input for continuous gesture tracking and translation.



User-Friendly Interface: Displays recognized signs and generated sentences with a clean OpenCV-based UI.

Tech Stack





Python: Core programming language for development.



TensorFlow Lite: Lightweight framework for deploying the transformer model.



OpenCV: Library for real-time video capture and visualization.



MediaPipe: Framework for hand, pose, and face landmark detection.



Gemini API: External API for generating coherent sentences from recognized ASL signs.



Pandas & NumPy: Used for data preprocessing and handling.



python-dotenv: Manages environment variables (e.g., API keys).

Setup and Testing

To run the project on your local machine, follow these steps:





Clone the Repository:

git clone https://github.com/yourusername/GISLR_sign-language.git
cd GISLR_sign-language



Install Dependencies:





Ensure Python 3.8+ is installed.



Install required packages:

pip install -r requirements.txt



If requirements.txt is not present, install manually:

pip install opencv-python mediapipe tensorflow pandas numpy python-dotenv requests



Set Up Environment Variables:





Create a .env file in the project root with your Gemini API key:

echo "GOOGLE_API_KEY=your_api_key_here" > .env



Replace your_api_key_here with your actual Gemini API key.



Ensure Webcam Access:





On Ubuntu, add your user to the video group to avoid permission issues:

sudo usermod -a -G video $USER



Log out and back in to apply changes.



Run the Application:





Execute the main script (replace app.py with your actual script name, e.g., main.py):

python app.py



The script will open a webcam feed, display recognized signs, and generate sentences when you press the Escape key.

Demo

For a visual demonstration of the project, check out the YouTube video (update with your demo link if available).

License

This project is licensed under the MIT License. See the LICENSE file for more information.

About

This repository contains a transformer-based model for real-time American Sign Language (ASL) recognition. It leverages a TensorFlow Lite model for gesture recognition and the Gemini API for sentence construction, enabling accessible communication through live video input.
