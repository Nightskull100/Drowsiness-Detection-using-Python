# Drowsiness Detection using Python

## Overview
This repository contains a Python script for detecting drowsiness using computer vision and facial landmarks. The system monitors the eyes' aspect ratio to identify signs of drowsiness and issues alerts when necessary.

## Requirements
- Python 3.x
- OpenCV
- imutils
- dlib
- pygame

## Installation
1. Install the required packages using:
   ```
   pip install opencv-python imutils dlib pygame
   ```

2. Download the pre-trained shape predictor model from [here](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2) and place it in the "models" folder.

## How to Use
1. Run the script by executing the following command in the terminal:
   ```
   python drowsiness_detection.py
   ```

2. The webcam will activate, and the system will start monitoring your eyes.

3. If drowsiness is detected, an alert message will be displayed on the video feed, and an alarm will be triggered.

4. To exit the application, press 'q'.

## Configuration
- Adjust the `thresh` variable to set the threshold for drowsiness detection.
- Modify the `frame_check` variable to determine the number of consecutive frames for triggering an alert.

## Credits
- The facial landmark detection is performed using the dlib library.
- The `FACIAL_LANDMARKS_68_IDXS` indices are used from the imutils library.

Feel free to contribute, report issues, or suggest improvements!
