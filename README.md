# Object Tracking with OpenCV

This repository contains a Python script for real-time object tracking using OpenCV. The script uses the **CSRT tracker** to track an object selected by the user in a video stream from a webcam.

## Features
- Real-time object tracking using a webcam feed.
- User-defined region of interest (ROI) for tracking.
- Visual feedback with a bounding box around the tracked object.
- Exit the program by pressing the `q` key.

## Requirements
To run this script, you need the following:
- Python 3.x
- OpenCV (`opencv-python`)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/AbdulrahmanRagab/object-tracking-opencv.git
   cd object-tracking-opencv
   ```

2. Install the required dependencies:
   ```bash
   pip install opencv-python
   ```

## Usage
1. Run the script:
   ```bash
   python object_tracking.py
   ```

2. When the webcam feed opens:
   - Select the object you want to track by drawing a bounding box around it using your mouse.
   - Press `Enter` to start tracking.

3. The script will track the selected object in real-time. A green bounding box will indicate the tracked object.

4. To exit the program, press the `q` key.

## Code Overview
The script performs the following steps:
1. Initializes the webcam feed using `cv2.VideoCapture`.
2. Allows the user to select a region of interest (ROI) using `cv2.selectROI`.
3. Initializes the CSRT tracker with the selected ROI.
4. Continuously updates the tracker and displays the tracked object with a bounding box.
5. Exits the program when the `q` key is pressed.
