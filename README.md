# Drowsiness-monitoring-Using-OpenCV
# Drowsiness Monitoring System

This project implements a drowsiness monitoring system using OpenCV and Tkinter. The system detects signs of drowsiness based on real-time facial feature analysis, providing a practical tool to enhance safety in environments such as driving or operating heavy machinery.

## Features

- **Real-Time Detection**: Monitors eyes and facial landmarks to assess drowsiness in real-time.
- **User-Friendly Interface**: Built using Tkinter for an easy-to-use graphical interface.
- **Alert System**: Triggers alerts when signs of drowsiness are detected.

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/VishnuPrakash01/Drowsiness-monitoring-Using-OpenCV.git
    cd drowsiness-monitoring
    ```

2. **Install Dependencies**:
    Ensure you have Python installed on your system, then run:
    ```bash
    pip install opencv-python opencv-contrib-python
    pip install numpy
    ```

    Tkinter is included with most Python installations. If not, install it using your package manager (e.g., `sudo apt-get install python3-tk` on Ubuntu).

3. **Download Haarcascade Files**:
    Download the required Haarcascade XML files for face and eye detection from the OpenCV GitHub repository:
    - [Haarcascade Frontal Face](https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml)
    - [Haarcascade Eye](https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_eye.xml)

    Save these files in the project directory.

## Usage

1. **Run the Application**:
    ```bash
    python drowsiness_monitoring.py
    ```

2. **Features of the Application**:
    - The GUI allows you to start and stop drowsiness detection.
    - Alerts are displayed and/or sounded when drowsiness is detected.

## Modules Used

- **Tkinter**: For creating the graphical user interface (GUI).
- **OpenCV**: For real-time video processing and facial feature detection.

## How It Works

1. **Face and Eye Detection**:
    - The system uses Haarcascade classifiers to detect faces and eyes in a video feed.

2. **Eye Aspect Ratio (EAR)**:
    - EAR is computed based on facial landmarks to determine if the eyes are closed for an extended period.

3. **Alert Mechanism**:
    - If EAR remains below a predefined threshold for a certain duration, the system triggers an alert.

## Contribution

Feel free to fork this repository and make improvements. Contributions are welcome through pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- OpenCV documentation and tutorials.
- Python community for the Tkinter module.

---

## Contact

For queries or support, please contact: [vishnu] vishnuprakashl0112@gmail.com

Stay safe and stay awake!
