Overview

This project is an American Sign Language (ASL) detection system that recognizes hand gestures using computer vision and machine learning and converts them into speech. The system uses Mediapipe for hand landmark detection, a pre-trained model for gesture classification, and Text-to-Speech (TTS) for converting recognized text into speech. The graphical user interface (GUI) is built using Tkinter.


![alt text](ReadmeAssets/ASL_&_custom_hand_sign.jpg)

Features

Real-time ASL detection using webcam

Hand landmark detection with Mediapipe

Machine learning-based gesture classification

Automatic word and sentence formation from detected gestures

Text-to-Speech (TTS) conversion for speaking out sentences

Graphical User Interface (GUI) for interaction

Pause, Reset, and Speak Sentence options

Project Workflow

Video Capture: The system captures video frames from the webcam.

Hand Detection: Mediapipe detects hand landmarks in the video frame.

Feature Extraction: The system extracts hand landmark coordinates.

Gesture Classification: A trained ML model predicts the ASL gesture.

Text Formation: Recognized gestures are formed into words and sentences.

Speech Conversion: The final sentence is converted into speech using TTS.

GUI Interaction: Users can view recognized gestures, sentences, and control the system via buttons.

File Structure

├── model.p            # Pre-trained machine learning model for ASL recognition
├── Main.py            # Main application script with video processing and GUI
├── README.md          # Project documentation

Installation

Prerequisites

Ensure you have Python installed (version 3.x recommended). Install dependencies using:

pip install -r requirements.txt

Required Libraries

OpenCV (cv2)

Mediapipe

Numpy

Tkinter (built-in in Python)

Pyttsx3 (for Text-to-Speech)

Pickle (for model loading)

Running the Project

To start the ASL detection system, run:

python Main.py

Usage

Show ASL gestures in front of the camera to recognize letters.

The system forms words and sentences automatically.

Press 'Speak Sentence' to convert the detected sentence into speech.

Use 'Pause' to stop recognition and 'Reset' to clear the sentence.