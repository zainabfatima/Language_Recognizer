# Language_Recognizer
This is a basic deep neural network model that can recognize three sign language gestures:

✋ "hello"

🙏 "thanks"

🤟 "iloveu"

The system:

Works in real time using OpenCV for video capture

Uses Mediapipe to detect and show hand landmarks

Classifies detected gestures using a pre-trained model (action.h5)

Allows adding more signs easily by expanding the training dataset and model

📂 Repository Structure

Basic-Sign_Language-Recognizer/
├── 0.npy                         # Preprocessed training data (landmarks/coords)
├── README.md                     # Project description
├── action.h5                     # Pre-trained deep learning model for gesture classification
├── original sign recognition.ipynb # Jupyter Notebook with full implementation
⚙️ How It Works
Capture Video – OpenCV captures the live video feed.

Detect Hand Landmarks – Mediapipe extracts key points of the hand.

Feature Processing – The coordinates are normalized and converted into a feature vector.

Gesture Classification – The pre-trained model (action.h5) predicts the gesture.

Real-time Display – Recognized gesture is displayed on the video frame.
