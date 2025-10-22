Webcam-Smile-detection

The steps of the webcam smile detection code are:

Import OpenCV library.

Load Haar cascade classifiers for face and smile detection.

Start the webcam video capture using cv2.VideoCapture(0).

Enter an infinite loop to read frames from the webcam.

Convert each frame to grayscale (Haar cascades work on grayscale).

Detect faces in the grayscale frame using the face cascade.

For each detected face, draw a blue rectangle on the color frame.

Define the face region of interest (ROI) in grayscale and color images.

Detect smiles within the face ROI using the smile cascade.

For each detected smile, draw a green rectangle and label with "Smile".

Display the video stream with the drawn rectangles.

Exit the loop and close windows when the 'q' key is pressed.

Release webcam resource and destroy all OpenCV windows.

These steps achieve real-time face and smile detection from webcam video using pretrained Haar cascades in OpenCV.​
