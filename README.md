# DeadLift_Counter App
This is a Python script that creates a GUI-based Deadlift Counter application using the Tkinter library. The app uses a pre-trained machine learning model to detect different stages of a deadlift and counts the number of repetitions completed.

## Requirements

This app requires the following libraries to be installed:

- tkinter
- customtkinter
- pandas
- numpy
- pickle
- mediapipe
- cv2
- PIL

## Usage

To use the app, simply run the script in a Python environment. The app will open up in a GUI window.

The GUI consists of three labels displaying the current stage of the deadlift, the number of repetitions completed, and the probability of the current stage. There is also a RESET button that resets the counter to zero.

The main part of the GUI is a video feed captured by the user's camera. The app uses a pre-trained machine learning model to detect different stages of the deadlift and counts the number of repetitions completed.

To exit the app, simply close the GUI window.

## Code Explanation

The app first imports the necessary libraries and sets up the GUI window. Different labels and a RESET button are placed on the window using customtkinter library. A frame is also placed to display the video feed.

A pre-trained machine learning model is loaded from a pkl file using the pickle library. The app captures the user's camera feed using cv2 and uses mediapipe library to detect different landmarks and stages of the deadlift.

The detect() function is used to detect the different stages of the deadlift and count the number of repetitions completed. The function captures the user's camera feed, detects the landmarks, and predicts the stage and probability using the pre-trained machine learning model.

The GUI is updated in real-time with the current stage, number of repetitions completed, and probability. The detect() function is called repeatedly to update the GUI continuously.

##Future Improvements

This app can be improved by adding a feature to save the data from each deadlift session. This could include the number of repetitions completed, the time taken to complete the session, and other useful metrics. The app could also be improved by adding more exercises and pre-trained machine learning models to detect them.
