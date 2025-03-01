# hand-detection-opencv-mediapipe
Real-time hand detection and tracking using OpenCV and Mediapipe. Detects hand landmarks, tracks positions, and displays FPS on a live video feed.

# Hand Detection using OpenCV and Mediapipe

## Overview
This project implements real-time hand detection and tracking using OpenCV and Mediapipe. The script captures video from a webcam, detects hands, and tracks key landmark positions, displaying them on the video feed. The frame rate (FPS) is also displayed.

## Features
- Detects hands in real-time.
- Draws hand landmarks and connections.
- Prints the thumb tip coordinates in the console.
- Displays FPS on the video feed.
- Closes when 'q' is pressed.

## Requirements
Make sure you have the following dependencies installed:

```sh
pip install opencv-python mediapipe
```

## Usage
1. Clone or download the repository.
2. Run the script using:

```sh
python hand_detection.py
```

3. The webcam will open, and detected hands will be displayed with landmarks.
4. Press 'q' to exit.

## Code Explanation
### `HandDetector` Class
- **`__init__`**: Initializes Mediapipe's hand detection model.
- **`findHands(img, draw=True)`**: Detects hands and draws landmarks.
- **`findPosition(img, results, draw=True)`**: Extracts and returns hand landmark positions.

### `main()` Function
- Captures video from the webcam.
- Uses `HandDetector` to detect hands.
- Prints the thumb tip coordinates.
- Displays FPS.
- Press 'q' to exit.

## Output
- **Console Output**: Displays coordinates of the thumb tip if detected.
- **GUI Output**: Webcam feed with hand landmarks and FPS displayed.

## Example Console Output
```
[320, 240]
[325, 245]
[330, 250]
```

## Example Screenshot
📷 *(Hand with key points marked and FPS displayed in the top-left corner)*

## License
This project is open-source and available under the MIT License.

