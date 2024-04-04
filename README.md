# 🖐️ AI-Powered Virtual Mouse

Welcome to the AI-Powered Virtual Mouse project! This project uses hand gestures to control the mouse cursor. It leverages OpenCV for capturing video frames, MediaPipe for hand detection, and PyAutoGUI for controlling the mouse.

## 🎯 Features

- **Real-time Hand Detection:** The application captures video feed in real-time and detects hand movements.
- **Mouse Control:** You can control the mouse pointer using your index finger.
- **Click Action:** Perform click actions by bringing your thumb and index finger close together.

## 📦 Modules Used

- `cv2`: The OpenCV library is used for capturing video frames and image processing.
- `mediapipe`: Google's MediaPipe library is used for hand detection.
- `pyautogui`: This library allows for programmatically controlling the mouse.

## 🚀 How to Run

1. Ensure you have Python installed on your machine.
2. Install the necessary libraries using pip:

```bash
pip install opencv-python
pip install mediapipe
pip install pyautogui
```
##  🏃 Run The File

To run the file run the main python file mouse.py

## ⚠️ Remainder

Please note that the system is currently in the early stages of development and may not be fully optimized.

## 📚 For More Detail

For a detailed explanation of the code, please refer to the comments in the code files. Each line of code is explained to help you understand how the program works.

## 🚧 Future Work

Add support for more gestures and map them to different functions.
Improve hand detection accuracy and robustness.
Add support for custom gestures defined by the user.

## 🤝 Contributions

Contributions to this project are welcome! Please fork the repository and open a pull request with your changes.

## 📄 License

This project is licensed under the MIT License. See the LICENSE file for more details.

## 🛠️ How It Works

The script starts by capturing video frames from the webcam using OpenCV. These frames are then passed to the hand detection model from the MediaPipe library. The model returns the positions of different landmarks on the hand. A yellow circle is drawn around the index finger and the thumb to show the position of the fingers being tracked. The script uses the position of the index finger to control the position of the mouse pointer. When the thumb and index finger come close together, a click action is performed.

![Hand Landmarks](data:image/png;base64,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)

The image above shows the landmark points in the hand which are used to detect the presence of the hand and also to control movement of the fingers.
