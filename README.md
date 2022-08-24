# Smile-Capture

## Discription
I create an automatic smile capture selfie. Here we used the system webcam, and our picture gets captured when we smile.

##  Library used

**OpenCV-Python**: OpenCV is an excellent tool for image processing and computer vision tasks. It is an open-source library that performs functions like face detection, objection tracking, landmark detection, and much more.
OpenCV-python used for computer vision, machine learning, and image processing.

**Datetime**: For work with date and time.

**Playsound**: For playsound in our program.

## Execution Steps:

1.	Import libraries.
2.	Then we record the video using our system camera(here, laptop front webcam) and VideoCapture(0). Here 0 is used to turn on our system webcam to record.
3.	Here, we provide the location to access our cascade file(face_cascade, smile_cascade). (Haarcascade is an Object Detection Algorithm used to identify faces in an image or a real-time video. The algorithm uses edge or line detection features. )
4.	We run a loop to read video (as we know, video is a set of collections of frames) and for performing functions.
5.	We use cvtColor to convert colour to greyscale to increase accuracy and use detectMultiScale to detect the faces. This function will return a rectangle with coordinates (x, y, w, h) around the detected face, and scaleFactor specifies the image size reduced with each scale.
6.	Then we run a for a loop; this function recognizes the face and smile.
7.	We use the rectangle function to draw a rectangle over a face that is detected and again use detectMultiScale.
8.	We use a nested for loop to put a rectangle on the smile(i.e., lips when in the smiling position).
9.	For saving the image with time and date in a specific format, we use datetime.datetime.now().strftime() and enter such a particular date and time format.
10.	Finally, the image (.png format) is stored in the working directory.




https://user-images.githubusercontent.com/72460920/186488913-ceb02513-3643-4d7d-9941-e6d71a544215.mp4


