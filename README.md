<h2>SeeThru: Real time webcam monitorting system.</h2>

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-Real--Time--Vision-red)
![YOLOv3](https://img.shields.io/badge/YOLOv3-Object--Detection-green)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

### Aim

To develop an **real monitoring system** capable of monitoring student behaviour during online tests through **real-time face and object detection**, ensuring exam integrity and minimizing manual supervision.

## Methodologies

| # | Methodology | Description |
|---|--------------|-------------|
| 1 | **OpenCV for Input Capture** | Captures live webcam feed and performs real-time face detection using Haar Cascades. |
| 2 | **YOLOv3 Object Detection** | Detects multiple object types simultaneously within the camera frame. |
| 3 | **Real-Time Processing** | Processes frames instantly to ensure live monitoring and feedback. |
| 4 | **Warning System** | Triggers alerts (sound + text) if the student is away or unauthorized items are detected. |
| 5 | **Data Logging** | Records events and stores them as terminal outputs or in PDF logs for later analysis. |

### Libraries 
~~~bash
OpenCV (cv2)
NumPy
Pygame
Time
OS
Subprocess
gTTS
Pydub
~~~

### Installation & Setup
1. Clone the repository
~~~bash
git clone https://github.com/your-username/student-behaviour-monitoring.git
cd student-behaviour-monitoring
~~~

2. Install dependencies
~~~bash
pip install opencv-python pygame numpy gtts pydub
~~~

3. Download assets from: 

4. Run the project:
~~~bash
python main.py
~~~

- [face_detection.py](face_detection.py) file uses cascade filters to detect the face and there is a threshold value of 5sec set in the function such that, if the user is not detected for more than 5sec it shoots an alert with buzzer sound.
- [object_detection.py](object_detection.py) file uses YOLO libraries to detect the objects that are present in the captured area and prints the objects with their respective positions in the terminal.
- We integrate the features of both [face_detection.py](face_detection.py) and [object_detection.py](object_detection.py) in [main.py](main.py).


