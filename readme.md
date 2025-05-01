Hand Gesture-Based Drawing & AI Integration

<!-- REQUIREMENT : python version 3.10 -->

-Overview

This project implements a hand gesture-based drawing system using MediaPipe, CVZone, and OpenCV for hand tracking. The system allows users to draw using gestures and integrates with Gemini AI to solve drawn mathematical problems. It includes both GUI and Non-GUI versions.


-Installation Prerequisite

Make sure you have Python installed and set up the following dependencies available in the code cells 

pip install opencv-python numpy mediapipe cvzone pillow google-generativeai numpy tkinter
<!-- you may need to restart the kernel to use updated packages -->


-Features

Hand Tracking & Drawing: Uses MediaPipe and CVZone to detect hands and recognize finger states.

-Gesture Controls:

--Index Finger Up ([0, 1, 0, 0, 0]) → Draws on the canvas.

--Peace Sign ([0, 1, 1, 0, 0]) → Pauses drawing to reset to null position which helps when we want gap or space between each characters.

--Pinky Down ([1, 1, 1, 1, 0]) → Sends the canvas to Gemini AI for problem-solving.

-AI Integration:

Captures the drawn image and sends it to Gemini AI.

The AI response is displayed in the console (Non-GUI) or Tkinter window (GUI).

-GUI vs. Non-GUI:

--Non-GUI: Fully gesture-controlled, AI response shown in the console.

--GUI: Provides button-based control and AI response is displayed in a window.



-Usage

-Running the Non-GUI Version

projectcv.ipynb 

-Running the GUI Version

projectcvUi.ipynb

-Controls

--Press 'c' → Clear the drawing canvas.

--Press 'q' → Exit the application.

In GUI version, use the Clear Canvas and Send AI buttons for additional control.

-Acknowledgments

--MediaPipe & CVZone for hand tracking.

--OpenCV for real-time image processing.

--Google Gemini AI for problem-solving integration.

-License

This project is licensed under the MIT License.

