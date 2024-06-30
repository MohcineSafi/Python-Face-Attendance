# Face Recognition Attendance System

This project is a face recognition attendance system built using Python and Tkinter. It leverages the `face_recognition` library to detect and recognize faces and the `Silent-Face-Anti-Spoofing` models to prevent spoofing attempts.

## Features

- **Login**: Recognize and authenticate users based on their facial features.
- **Logout**: Record the logout time of authenticated users.
- **Register New User**: Add new users to the system by capturing their facial features.
- **Real-Time Webcam Feed**: Continuously capture images from the webcam for real-time face recognition.

## Requirements

- Python 3.x
- OpenCV
- face_recognition
- Pillow
- Tkinter

## Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/yourusername/face-recognition-attendance-system.git
   cd face-recognition-attendance-system
   ```

2. **Install dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

   Ensure `requirements.txt` includes:

   ```text
   opencv-python
   face_recognition
   pillow
   ```

3. **Download Anti-Spoofing Models**:

   Download the Silent-Face-Anti-Spoofing models and place them in the appropriate directory.

## Usage

1. **Run the Application**:

   ```bash
   python main.py
   ```

2. **Login**:

   - Click on the `login` button.
   - The system will capture your image, perform anti-spoofing checks, and recognize you based on the registered data.
   - If recognized, it logs the time of login.

3. **Logout**:

   - Click on the `logout` button.
   - The system will capture your image, perform anti-spoofing checks, and recognize you based on the registered data.
   - If recognized, it logs the time of logout.

4. **Register New User**:

   - Click on the `register new user` button.
   - A new window will open to capture the image and input the username.
   - Click `Accept` to register the user.

## File Descriptions

- **main.py**: The main application script. It sets up the Tkinter GUI, handles user interactions, and integrates the face recognition and anti-spoofing functionalities.
- **util.py**: Utility script containing helper functions for GUI components, face recognition, and message boxes.
- **db/**: Directory where user face embeddings are stored as `.pickle` files.
- **log.txt**: Log file to keep track of user login and logout times.

## Notes

- Ensure that your webcam is connected and accessible.
- The anti-spoofing model should be correctly placed in the specified directory in `main.py`.
