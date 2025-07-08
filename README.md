 Hand Gesture Recognition using Python and OpenCV
Overview:
Developed a real-time hand gesture recognition system capable of detecting and classifying four common hand gestures—Waving, Pointing, Scissors, and Rock—through a webcam interface using Python and OpenCV.

Key Features:

Real-time Video Processing: Captures and processes live video stream using OpenCV's VideoCapture, with mirroring for intuitive user interaction.

Background Subtraction: Implements adaptive background averaging and differencing to isolate the hand from the environment, using grayscale conversion and Gaussian blurring for noise reduction.

Region of Interest (ROI): Focuses processing on a specific screen segment to optimize performance and reduce false positives.

Hand Tracking Class: Defines a HandData object to store bounding box coordinates, movement history, finger count, and gesture state.

Gesture Detection Pipeline:

Waving Detection: Tracks horizontal palm movement over time using contour center shifts and convex hull bounding box.

Finger Counting: Draws a virtual line below finger tips and detects contour intersections to estimate number of extended fingers.

Gesture Smoothing: Aggregates recent frame predictions and selects the most frequent to improve stability and reduce jitter.

Visual Feedback: Overlays text and bounding boxes directly on the video feed to indicate gesture recognition status in real time.

Technologies Used:
Python, OpenCV, NumPy

Applications:
Human-computer interaction, touchless interfaces, basic sign language recognition, accessibility tools.
