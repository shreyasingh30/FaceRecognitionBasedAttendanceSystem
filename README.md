# FaceRecognitionBasedAttendanceSystem

To maintain the attendance record with day to day activities is a challenging task. The conventional method of calling
name of each student is time consuming and there is always a chance of proxy attendance. The following system is based
on face recognition to maintain the attendance record of students.

**Libraries needed**
1. cmake
2. dlib
3. face_recognition
4. numpy
5. opencv-python

**How to do it?**

1.Loading Images from an folder and Converting to RGB.
2.Compute the encodings for all the images.
3.Capture frames from webcam.
4.Once we have the webcam frame we will find all the faces in our image. The face_locations function is used for this purpose. Later we will find the face_encodings as well.
5.Now we can match the current face encodings to our known faces encoding list to find the matches. We will also compute the distance. 
6.Once we have the list of face distances we can find the minimum one, as this would be the best match.
7.Mark attendance in the csv file of the best match.

