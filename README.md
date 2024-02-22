Head Pose Estimation using MediaPipe and OpenCV

Introduction:

This Python script demonstrates head pose estimation using the MediaPipe library and OpenCV. It tracks facial landmarks in real-time, calculates the rotation angles of the head, and determines the direction in which the user is looking (left, right, up, down, or forward).

Requirements:

->Python 3.x

->OpenCV

->MediaPipe

->NumPy

Installation:

->Install Python (if not already installed) from python.org.

->Install OpenCV using pip:
    
    pip install opencv-python

->Install MediaPipe using pip:

    pip install mediapipe

Usage:

Ensure your webcam is connected and properly functioning.

Run the script by executing the command:

    python head_pose_estimation.py

The webcam window will open, showing your face with overlaid annotations.
The annotations display the direction in which your head is tilted and the estimated FPS (Frames Per Second) in the top-left corner of the window.

Description:

The script utilizes the MediaPipe Face Mesh model to detect facial landmarks such as the nose, eyes, and mouth.
It calculates the 3D coordinates of specific landmarks on the face.
Using the solvePnP function from OpenCV, it estimates the rotation and translation vectors of the head.
It then extracts the rotation angles from the rotation matrix.
Based on the rotation angles, the script determines whether the user is looking left, right, up, down, or forward.
The estimated head pose and FPS are displayed in real-time on the webcam feed.

References:

MediaPipe: https://google.github.io/mediapipe/

OpenCV Documentation: https://opencv.org/
