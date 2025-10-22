Webcam-Smile-detection

This code performs face and eye detection on a given image using OpenCV's Haar Cascade classifiers.

Description of the Code
Step 1: Load Haar Cascade classifiers
The code loads pre-trained Haar Cascades for detecting faces (haarcascade_frontalface_default.xml) and eyes (haarcascade_eye.xml) from OpenCV’s data directory.

Step 2: Read and preprocess the image
It reads an image ("Addision.jpg") and converts it to grayscale since Haar Cascade detection works on grayscale images.

Step 3: Detect faces
Using the face cascade, it detects faces in the grayscale image with specified parameters: scaleFactor (scale at which image size is reduced), minNeighbors (how many neighbors each candidate rectangle must have to retain), and minSize (minimum size of detected face).

Step 4: Draw rectangles around detected faces
For each detected face, the code draws a blue rectangle on the original color image indicating face boundaries.

Step 5: Detect eyes within each detected face
In the face region of interest, it applies the eye cascade to detect eyes and draws green rectangles around detected eyes inside the face.

Step 6: Display the image with detection rectangles
Finally, it shows the resulting image in a window titled "Face and Eyes Detection". The window waits indefinitely for a key press before closing.
