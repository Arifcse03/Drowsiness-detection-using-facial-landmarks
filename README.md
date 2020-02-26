# Drowsiness-detection-using-facial-landmarks
This project will help the driver to stay alert while driving. 
This is focused on drowsy driver detection and the objective of this thesis is to recognize a driver’s state with high performance. The general flow of our drowsiness detection methods is fairly straightforward. First, we’ll set up a camera that monitors a stream for the face. Here the face will be detected by using Histograms of Oriented Gradient & Linear SVM [1]. If a face is found, we apply facial landmark detection [2] and extract the eye regions. Now that we have the eye regions, we can compute the eye aspect ratio [3] to determine if the eyes are closed. If the eye aspect ratio indicates that the eyes have been closed for a sufficiently long enough amount of time, we’ll sound an alarm to wake up the driver.
There are two main states of a driver, those are alert and drowsy states. Video segments captured are analyzed by making use of image processing techniques. Eye regions are detected and those eye regions are input to right and left eye region classifiers, which are implemented using Histograms of Oriented Gradient & Linear SVM [1].
The eye states along the video segment are fused and the driver’s state is predicted as alert or drowsy. The proposed method is tested on 30-second- long video segments. The aim is to indicate that the planned technique has achieved better accuracy

For the project, we will need
1.openCV
2.imutils
3.dlib
4.scipy
5.Numpy
