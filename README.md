# Interactive LED Control using Python and Arduino

## Project Overview
This project enables **real-time interactive LED control** using **hand gestures** detected via a webcam. It integrates **Python (OpenCV, CVZone, Mediapipe)** with **Arduino** to translate finger movements into LED commands.

## Features
- **Hand Gesture Detection:** Uses OpenCV and Mediapipe to recognize the number of fingers displayed.
- **Arduino LED Control:** Sends signals to an Arduino to control LED states accordingly.
- **Real-Time Interaction:** Provides immediate feedback based on detected gestures.

## Technologies Used
- **Python** (for image processing and gesture detection)
- **OpenCV** & **CVZone** (for image analysis)
- **Mediapipe** (for hand tracking)
- **Arduino** (for LED control)

## Installation & Setup
### Prerequisites
- Python 3.x installed
- Arduino IDE installed
- Required Python Libraries: OpenCV, Mediapipe, CVZone, pyserial
- Arduino board with LEDs connected

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/interactive-led-control.git
   cd interactive-led-control
   ```
2. Install dependencies:
   ```bash
   pip install opencv-python mediapipe cvzone pyserial
   ```
3. Upload the Arduino code to your board using the Arduino IDE.
4. Run the Python script to start gesture detection:
   ```bash
   python led_control.py
   ```

## How It Works
1. **Camera Captures Hand Gestures:**
   - The webcam detects the user’s hand.
2. **Finger Count is Analyzed:**
   - Mediapipe processes the image and counts extended fingers.
3. **Command is Sent to Arduino:**
   - Based on the count, a signal is sent via Serial communication.
4. **LEDs Respond to Gestures:**
   - The Arduino interprets the signal and controls the LEDs accordingly.

## Gesture Mapping
| Fingers Shown | LED Action        |
|--------------|-----------------|
| 0            | All LEDs OFF     |
| 1            | LED 1 ON         |
| 2            | LED 2 ON         |
| 3            | LED 3 ON         |
| 4            | LED 4 ON         |
| 5            | All LEDs ON      |

## Future Improvements
- Add **color selection** for LEDs using gestures.
- Improve gesture recognition accuracy.
- Develop a GUI for easier interaction.

## Contributors
- **Your Name**
- **Your Team (if any)**

## License
This project is licensed under [Your Preferred License].

---

For any issues or contributions, feel free to open an issue or submit a pull request on [GitHub](https://github.com/your-repo/interactive-led-control).

