# Air Canvas

Air Canvas is an interactive Python application that allows you to draw in the air using hand gestures captured by your webcam. This project uses computer vision techniques and hand tracking to create a virtual drawing experience.

## Features

- Draw in four different colors: Blue, Green, Red, and Yellow
- Clear canvas option
- Real-time hand tracking and gesture recognition
- Intuitive color selection interface

## Requirements

- Python 3.x
- OpenCV (cv2)
- NumPy
- Mediapipe

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/abbasmithaiwala/air-canvas
   cd air-canvas
   ```

2. Install the required dependencies:
   ```
   pip install opencv-python numpy mediapipe
   ```

## Usage

1. Run the script:
   ```
   python air_canvas_ml.py
   ```

2. A window will open showing the webcam feed and the canvas.

3. Use your index finger to draw. The tip of your index finger acts as the drawing point.

4. To select a color or clear the canvas, move your index finger to the corresponding button at the top of the screen.

5. To stop drawing (lift the pen), bring your thumb close to your index finger.

6. Press 'q' to quit the application.

## How it Works

- The application uses Mediapipe for hand tracking.
- It identifies the position of your index finger and thumb.
- When your index finger is detected, it starts drawing on both the video feed and a separate canvas.
- The color selection and clear functionalities are triggered by moving your index finger to the respective areas at the top of the screen.
- The drawing is paused when your thumb and index finger are close together, simulating lifting a pen.

## Customization

You can modify the following aspects of the project:

- Change colors by modifying the `colors` list in the script.
- Adjust the canvas size by changing the dimensions in the `paintWindow` initialization.
- Modify gesture recognition sensitivity by tweaking the distance threshold between the thumb and index finger.

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/yourusername/air-canvas/issues) if you want to contribute.

## License

[MIT](https://choosealicense.com/licenses/mit/)
