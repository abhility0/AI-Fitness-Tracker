__**AI-Fitness-Tracker**__

_*Overview*_
The Workout Correction System is a real-time application designed to assist users in maintaining correct form during various exercises. It utilizes the MediaPipe library for pose estimation and OpenCV for video processing. The system can track and count repetitions for exercises such as squats, lat raises, bicep curls, push-ups, shoulder presses, and sit-ups, ensuring that users perform exercises with the correct posture.

*Features*
- Real-Time Pose Detection: Uses MediaPipe to detect body landmarks and track user movements.
- Exercise-Specific Tracking: Monitors angles between joints to assess form for different exercises.
- Repetition Counting: Counts repetitions automatically based on user movements and angle thresholds.
- User Interface: Simple GUI for selecting exercises and starting the workout session.

*Requirements*
- Python 3.x
- OpenCV
- MediaPipe
- Numpy
- Tkinter
- PIL (Pillow)

*Installation*

Clone the Repository 

Install Dependencies: Use pip to install the required Python libraries:
pip install opencv-python mediapipe numpy pillow

*Usage*
Run the Application:
python workout_correction_system.py

Select an Exercise:
The application will open with a GUI where you can select the exercise you want to perform.

Start Workout:
The webcam feed will be displayed with real-time pose detection.
Perform the selected exercise in front of the camera. The system will monitor your form and count repetitions automatically.
End Session:

After completing your workout, close the video window to end the session.

*How It Works*
- Pose Detection: The application captures video input from your webcam and processes it using MediaPipe's pose estimation model.
- Angle Calculation: The angle between specific joints is calculated to determine the current stage of the exercise (e.g., "up" or "down").
- Repetition Counting: The system counts a repetition when the user completes a full range of motion based on predefined angle thresholds.
- Real-Time Feedback: The current repetition count and stage are displayed on the video feed, providing immediate feedback on your workout.
