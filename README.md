Driver Drowsiness Detection System

Project Overview

This project detects driver drowsiness in real-time using computer vision techniques and a webcam. It monitors facial features such as eye closure and yawning to identify signs of fatigue and alert the user, helping prevent accidents.

Tech Stack

1)Python

2)OpenCV

3)MediaPipe

4)NumPy


Key Features

1)Real-time face tracking using webcam

2)Eye closure detection using Eye Aspect Ratio (EAR)

3)Yawning detection using Mouth Aspect Ratio (MAR)

4)Two detection modes:

    Eye-only detection
    EAR + MAR combined detection for improved accuracy
    
5)Visual alert system when drowsiness is detected


Methodology

1. Eye-Only Detection

   Uses Eye Aspect Ratio (EAR) to monitor eye state
   
   If EAR falls below a threshold, eyes are considered closed
   
   Continuous eye closure triggers drowsiness alert

2. EAR + MAR Detection

Uses EAR for eye closure detection

Uses Mouth Aspect Ratio (MAR) to detect yawning

Combines both signals to improve detection accuracy

Project Structure

 drowsiness_eye_only.py
 
 drowsiness_ear_mar.py
 
 README.md

Thresholds Used

EAR Threshold: 0.25 (eye closure detection)

MAR Threshold: 0.6 (yawning detection)

These values can be adjusted based on user behavior and lighting conditions.


How to Run

1. Install dependencies:
   pip install opencv-python mediapipe numpy

2. Run Eye-only detection:
   python drowsiness_eye_only.py

3. Run EAR + MAR detection:
   python drowsiness_ear_mar.py

4. Ensure webcam is enabled

Output

The system opens the webcam and tracks the user's face
  
Detects eye closure and yawning in real-time
  
Displays an alert on screen when drowsiness is detected


Applications

Driver safety systems

Accident prevention

Smart vehicle monitoring systems


Future Improvements

Add audio alert system for stronger warning

Improve detection accuracy using deep learning

Integrate with IoT-based vehicle systems

Deploy as a real-time application


Conclusion

This project demonstrates how computer vision techniques like EAR and MAR can be effectively used to detect driver drowsiness in real-time and enhance road safety.

