
# Drowsiness Detection System

The Drowsiness Detection System is designed to monitor a person's eye behavior using a webcam in real-time. The system utilizes facial landmark detection and the Eye Aspect Ratio (EAR) to identify signs of drowsiness or fatigue. When the system detects that the person's eyes have been closed for an extended period, it triggers an alert to notify the user, making it a valuable tool for preventing accidents caused by drowsy driving or fatigue-related tasks.


## DEPENDENCIES 
- `scipy`: Used for the Euclidean distance calculation in the eye_aspect_ratio function.
- `imutils`: Provides convenience functions for resizing and displaying images.
- `pygame`: Utilized for playing an alert sound when drowsiness is detected.
- `dlib`: A toolkit for machine learning and computer vision, used for face detection and landmark prediction.
- `OpenCV`: A computer vision library, used for video capture, image processing, and displaying results.

## PREREQUISITES 
- Make sure you have **Python** installed on your machine.
- Install the required dependencies using the following command: 
```bash
pip install scipy

pip install imutils

pip install pygame

pip install dlib

pip install opencv-python
```

## DEMO

The script will use your default webcam to monitor your eyes.
When signs of drowsiness are detected (prolonged eye closure), an alert will be triggered (e.g., a sound notification).

Press **'q'** to exit the application.
## PARAMETERS

`thresh`: Threshold for the Eye Aspect Ratio (EAR) below which an alert is triggered.

`frame_check`: Number of consecutive frames with EAR below the threshold to trigger the alert.
## TARGET AUDIENCE 

- **Drivers:** Especially long-distance drivers who may face the risk of drowsy driving.
- **Operators of Heavy Machinery:** Individuals operating heavy machinery or equipment where alertness is crucial for safety.
- **Office Workers:** Professionals spending extended hours in front of computers, ensuring they take breaks to avoid fatigue.

## Face and Eye Detection Scripts

### face_and_eye_detector_single_image.py
This script detects faces and eyes in a single image.Detects face and eye from a single image. Demo-

### Usage
- Download the shape predictor model file (`shape_predictor_68_face_landmarks.dat`) from dlib's official website and place it in the same directory as the script.
- Set the correct file path for the alert sound in the mixer.music.load function.
- Run the script.
