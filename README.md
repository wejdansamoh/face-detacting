# face-detacting
BY openCV and Python 
![an example](https://github.com/user-attachments/assets/e92fe78a-3729-4911-bd48-61aabb6a7c31)

Here's a simple Python script that uses OpenCV to detect a face in real-time using your webcam. 

This code utilizes the Haar Cascade Classifier, which is a popular method for face detection .

Explanation:
Loading the Haar Cascade Classifier:

The classifier is loaded using cv2.CascadeClassifier. The Haar Cascade XML file (haarcascade_frontalface_default.xml) is included with OpenCV and is used to detect faces.
Capturing Video:

The video feed is captured from the webcam using cv2.VideoCapture(0).
Grayscale Conversion:

The video frame is converted to grayscale because the Haar Cascade works with grayscale images.
Face Detection:

detectMultiScale() detects objects (in this case, faces) of different sizes in the input image. The detected objects are returned as a list of rectangles.
Drawing Rectangles:

For each face detected, a green rectangle is drawn around the face using cv2.rectangle().
Displaying the Frame:

The frame with the detected faces is displayed in a window titled "Video".
Loop Exit:

The loop will break when the 'q' key is pressed.
Cleanup:

The webcam is released, and all OpenCV windows are closed.
How to Run the Code:
Make sure you have OpenCV installed. You can install it using pip if you don't have it:

pip install opencv-python
