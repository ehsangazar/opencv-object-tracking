# OpenCV-Object-Tracking

You can read my article here

[https://ehsangazar.com/object-tracking-with-opencv-fd18ccdd7369](https://ehsangazar.com/object-tracking-with-opencv-fd18ccdd7369)

## What is Object Tracking ?

Simply put, locating an object in successive frames of a video is called tracking.
Usually tracking algorithms are faster than detection algorithms. The reason is simple. When you are tracking an object that was detected in the previous frame, you know a lot about the appearance of the object.
You also know the location in the previous frame and the direction and speed of its motion.
If you are running a face detector on a video and the person's face get's occluded by an object, the face detector will most likely fail. A good tracking algorithm, on the other hand, will handle some level of occlusion.
One of the famous libraries for tracking is OpenCV. 
OpenCV (Open Source Computer Vision) is a library of programming functions mainly aimed at real-time computer vision.[1] Originally developed by Intel,

## How to install OpenCV on Mac OS? 
Simple, you have probably python installed, so use brew to install opencv.
brew install opencv
pip3 install numpy
Then I used this video which is a short cut of Chaplin for doing object tracking, I am trying to track his face while he is dancing and turning around.
Normally the objects we are tracking would not be disappeared, but in this case for comparing different methods provided by OpenCV, I used this video.
Firstly importing cv2
```
import cv2
```
Then, 
```
tracker_types = ['BOOSTING', 'MIL','KCF', 'TLD', 'MEDIANFLOW', 'CSRT', 'MOSSE']
```

## Conclusion
If you are looking for solving tracking object in videos, OpenCV is one of the best, there are different algorithms which based on you scenario might work better.