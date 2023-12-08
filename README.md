---

# Drowsiness Detector

## Overview

The Drowsiness Detector is a Python script that utilizes facial landmarks and eye aspect ratio to detect signs of drowsiness in a person's eyes. It uses the dlib library for facial landmark detection and OpenCV for capturing and processing video frames.

## Requirements

- Python 3.x
- OpenCV
- dlib
- imutils
- winsound

## Installation

1. Install the required Python packages:

    ```bash
    pip install opencv-python dlib imutils
    ```

2. Download the shape_predictor_68_face_landmarks.dat file from [dlib.net](http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2) and place it in the project directory.

## Usage

Run the script by executing the following command in your terminal:

```bash
python drowsiness_detector.py
```

Press 'q' to exit the application.

## Algorithm

The script calculates the Eye Aspect Ratio (EAR) for both eyes, and if the average EAR falls below a certain threshold for a specified number of consecutive frames, it triggers an alert indicating potential drowsiness.

## Configuration

You can adjust the following parameters in the script:

- `earThresh`: Threshold for the Eye Aspect Ratio, indicating the distance between vertical eye coordinates.
- `earFrames`: Consecutive frames for eye closure to trigger a drowsiness alert.

## Credits

- [dlib](http://dlib.net/): A toolkit for making real-world machine learning and data analysis applications.
- [OpenCV](https://opencv.org/): Open Source Computer Vision Library.
- [imutils](https://github.com/jrosebr1/imutils): A series of convenience functions to make basic image processing operations such as translation, rotation, resizing, and displaying images easier with OpenCV.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
