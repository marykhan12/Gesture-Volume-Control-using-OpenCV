# Gesture-Volume-Control-using-OpenCV

This project demonstrates a gesture-based volume control system using hand tracking. The application leverages **OpenCV** for real-time camera input, **MediaPipe** for hand tracking, and **PyCaw** for audio control. The `HandTrackingModule.py` file is used to implement the hand tracking functionality, and the project's main script integrates gesture recognition with system volume adjustments.

---

## Features
- **Real-time Hand Detection**: Tracks hand landmarks using MediaPipe.
- **Gesture Control**: Uses the distance between thumb and index finger to adjust system volume.
- **Dynamic Feedback**: Visual representation of gestures and the current volume level.
- **Cross-Platform**: Compatible with systems that support OpenCV, PyCaw, and MediaPipe.

---

## Requirements
To run the project, ensure you have the following installed:

### Python Libraries:
- `opencv-python`
- `mediapipe`
- `pycaw`

### Install using pip:
```bash
pip install opencv-python mediapipe pycaw
```

---

## How It Works
1. **Hand Tracking**:
   - The `HandTrackingModule.py` detects hand landmarks in real-time using a webcam.
   - The distance between the tip of the thumb and the tip of the index finger is calculated.

2. **Volume Adjustment**:
   - The PyCaw library interacts with the system's audio endpoint to adjust volume based on the gesture.

3. **Visualization**:
   - Hand landmarks and the distance measurement are visualized on the webcam feed for user feedback.

---

## Project Structure
- **`HandTrackingModule.py`**: 
  A module for detecting hand landmarks and calculating distances between points.

- **`main.py`**:
  Contains the core logic for integrating gesture recognition with volume control.

---

## Setup and Usage
1. Clone or download the repository.
2. Place `HandTrackingModule.py` in the same directory as `main.py`.
3. Run the `main.py` script:
   ```bash
   python main.py
   ```
4. Use the following gestures to control volume:
   - **Join Thumb and Index Finger**: Adjust the distance to increase or decrease volume.
   - **Stretch Fingers**: Maximum volume.
   - **Close Fingers**: Minimum volume.


---

## Visualization
- A video feed with hand landmarks.
- Volume control displayed as a percentage on the screen.
- Bar indicator for volume level.

---

## References
- **OpenCV**: For camera input and visualization.
- **MediaPipe**: For robust hand landmark detection.
- **PyCaw**: For seamless audio endpoint volume control.

---

Feel free to customize or enhance the project! If you encounter issues, feel free to open a discussion. 🎉
