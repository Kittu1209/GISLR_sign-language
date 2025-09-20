# GISLR_sign-language: Real-Time ASL Recognition with Transformer Model

This repository contains a transformer-based model for real-time American Sign Language (ASL) recognition. The model leverages a state-of-the-art transformer architecture to interpret ASL gestures from live video input and integrates the Gemini API to construct coherent English sentences from recognized signs. This project aims to enhance communication accessibility for ASL users.

## Project Overview

The `GISLR_sign-language` project provides a robust solution for real-time ASL recognition. It captures live video using OpenCV, processes gestures with MediaPipe’s holistic tracking, predicts signs using a TensorFlow Lite transformer model, and generates meaningful sentences via the Gemini API. The system is designed for seamless, on-the-fly translation of ASL gestures into text, making it a valuable tool for communication.

## Features

- **Real-Time ASL Recognition**: Detects and recognizes ASL gestures in real-time from video input.
- **Transformer Architecture**: Utilizes a lightweight TensorFlow Lite transformer model for high-accuracy sign prediction.
- **Sentence Construction**: Integrates the Gemini API to form grammatically correct English sentences from recognized ASL words.
- **Live Video Input**: Supports webcam input for continuous gesture tracking and translation.
- **User-Friendly Interface**: Displays recognized signs and generated sentences with a clean OpenCV-based UI.

## Tech Stack

- **Python**: Core programming language for development.
- **TensorFlow Lite**: Lightweight framework for deploying the transformer model.
- **OpenCV**: Library for real-time video capture and visualization.
- **MediaPipe**: Framework for hand, pose, and face landmark detection.
- **Gemini API**: External API for generating coherent sentences from recognized ASL signs.
- **Pandas & NumPy**: Used for data preprocessing and handling.
- **python-dotenv**: Manages environment variables (e.g., API keys).

## Setup and Testing

To run the project on your local machine, follow these steps:

1. **Clone the Repository**:
   ```bash
   gh repo clone Kittu1209/GISLR_sign-language
   cd GISLR_sign-language

2. **Install Dependencies**

   Ensure Python 3.8+ is installed. Install required packages:

3. **Set Up Environment Variables**

   Create a `.env` file in the project root with your Gemini API key:

   ```bash
   echo "GOOGLE_API_KEY=your_api_key_here" > .env

   ```bash

4. **Ensure Webcam Access**

   On Ubuntu, add your user to the `video` group to avoid permission issues:

   ```bash
   sudo usermod -a -G video $USER

5. **Run the Application**

   Execute the main script (replace `main.py` with your actual script name if different):

   ```bash
   python main.py

## About

This repository contains a transformer-based model for real-time Google Isolated American sign language (ASL) recognition. It leverages a TensorFlow Lite model for gesture recognition and the Gemini API for sentence construction, enabling accessible communication through live video input.

