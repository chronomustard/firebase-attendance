# Firebase Attendance System

The Firebase Attendance System automates attendance tracking using facial recognition, built with OpenCV and Python. It's a modified iteration derived from [coneypo's Dlib_face_recognition_from_camera](https://github.com/coneypo/Dlib_face_recognition_from_camera), incorporating aspects from [Arjit1080's Face Recognition Based Attendance System](https://github.com/Arijit1080/Face-Recognition-Based-Attendance-System).

## Overview

The system simplifies attendance marking by employing facial recognition technology. It captures images via a connected camera, matches them against an existing database, and records attendance based on recognized faces.

## Installation

### Prerequisites

Ensure the following prerequisites are installed:

- **Python >= 3.7**
- **dlib == 19.17.0**
- **numpy == 1.22.0**
- **scikit-image == 0.18.3**
- **pandas == 1.3.4**
- **opencv-python == 4.5.4.58**
- **flask**
- **tkinter**
- **pillow**

### Installation Steps

1. Clone this repository to your local machine:
    ```bash
    git clone https://github.com/chronomustard/firebase-attendance
    ```

2. Install necessary packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Obtain the required dlib models from the [Google Drive link](https://drive.google.com/drive/folders/12It2jeNQOxwStBxtagL1vvIJokoz-DL4?usp=sharing) and place the 'data' folder within the cloned repository. This is essential in case the dlib models from the git repository are corrupted or inaccessible.

### Additional Installation Notes

- **Windows**: For dlib installation on Windows, download it from [sachadee/Dlib](https://github.com/sachadee/Dlib), ensuring compatibility with your Python version (3.7, 3.8, or 3.9). Consider using conda for a smoother installation process.
  
- **Linux**: Follow [this guide](https://pyimagesearch.com/2018/01/22/install-dlib-easy-complete-guide/) for dlib installation on Linux.

## Usage

1. Collect Faces Dataset:
    ```bash
    python get_faces_from_camera_tkinter.py
    ```

2. Convert the dataset:
    ```bash
    python features_extraction_to_csv.py
    ```

3. Record attendance:
    ```bash
    python attendance_taker.py
    ```

4. Database verification:
    ```bash
    python app.py
    ```

## Contributing

Contributions are welcome! If encountering bugs or having improvement suggestions, feel free to open an issue or submit a pull request.
