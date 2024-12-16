# Virtual-Keyboard

This project is a virtual keyboard application that utilizes hand gesture detection to simulate keypresses. It uses a webcam to detect hand movements, tracks finger positions, and triggers corresponding keyboard inputs in real-time.

## Features

- **Gesture Detection**: Detects finger positions using hand-tracking technology.
- **Virtual Keyboard**: A visual keyboard layout is displayed on the screen.
- **Simulated Keypresses**: Interact with the keyboard by pointing and pinching with your fingers.
- **Special Keys**: Includes support for `SPACE`, `ENTER`, and `BACKSPACE`.
- **Interactive UI**: Highlights keys when hovered or pressed.

## Requirements

The following libraries are required to run this project:

- `opencv-python`
- `cvzone`
- `numpy`
- `mediapipe`
- `pynput`

Install the required libraries using pip:

```bash
pip install opencv-python cvzone numpy mediapipe pynput
```

## How It Works

1. **Hand Detection**: Detects hand landmarks using `cvzone` and `MediaPipe`.
2. **Button Interaction**: Checks if the index finger is hovering over a key and simulates a key press when pinched with the thumb.
3. **Visual Feedback**: Highlights keys on hover and displays visual confirmation on key press.

## Usage

1. **Run the Script**
   Execute the script in your Python environment:

   ```bash
   python virtual_keyboard.py
   ```

2. **Interacting with the Virtual Keyboard**:
   - Open the application window.
   - Point at a key using your index finger.
   - Pinch your thumb and index finger to press the key.
   - Use special keys (`SPACE`, `ENTER`, `BACKSPACE`) as needed.
   - Press the `ESC` key to exit the application.

## Keyboard Layout

The virtual keyboard consists of the following layout:

```
1  2  3  4  5  6  7  8  9  0
Q  W  E  R  T  Y  U  I  O  P
A  S  D  F  G  H  J  K  L  ;
Z  X  C  V  B  N  M  ,  .  /
[SPACE] [ENTER] [BACKSPACE]
```

## Limitations

- Requires a high-quality webcam for accurate hand tracking.
- Performs best in well-lit environments.
- May have difficulties differentiating between multiple hands or unintended gestures.

## Future Enhancements

- Add multi-hand support for collaborative typing.
- Improve gesture recognition for smoother interactions.
- Include additional gestures for functionalities like copy, paste, or undo.
- Enhance the visual interface for better usability.

## Author

Parth Lathiya
