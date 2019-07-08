# SFND 2D Feature Tracking

This project is the second in a series for Udacity's Sensor Fusion Nanodegree. The project covers the following key concepts:

- Using ring buffers to avoid memory bloat while processing a sequence of images
- Keypoint detectors such as: Shi-Tomasi, Harris, FAST, BRISK, ORB, AKAZE, and SIFT
- Keypoint descriptor extraction and matching with: FLANN and k-NN

These techniques provide a foundation for the next step: time-to-collision estimation.

## Visualization of the results
<img src="images/sift-keypoints.png" width="903" height="339" />

## Overview of the workflow
1. Load the images into a ring buffer. 
1. Use OpenCV to apply a variety of keypoint detectors.
  - Shi-Tomasi
  - Harris
  - FAST
  - BRISK
  - ORB
  - AKAZE
  - SIFT (Patent encumbered, https://patents.google.com/patent/US6711293B1/en)
<!-- 1. Use FLANN and kNN to improve on the brute force matching of keypoint descriptors. -->
<!-- 1. Finally, run these algorithms in various combinations to compare performance benchmarks.  -->

It's important to distinguish between the terms of art keypoint **detector** and keypoint **descriptor**. From Udacity's lecture notes:
> - A keypoint (sometimes also interest point or salient point) detector is an algorithm that chooses points from an image based on a local maximum of a function, such as the "cornerness" metric we saw with the Harris detector.
> - A descriptor is a vector of values, which describes the image patch around a keypoint. There are various techniques ranging from comparing raw pixel values to much more sophisticated approaches such as histograms of gradient orientations.

## Dependencies
* cmake >= 2.8
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* OpenCV >= 4.1
  * On macOS, simply `brew install opencv`
  * If compiled from source, ensure that cmake flag is set `-D OPENCV_ENABLE_NONFREE=ON` for testing the SIFT and SURF detectors.
  * The OpenCV 4.1.0 source code can be found [here](https://github.com/opencv/opencv/tree/4.1.0)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

## Building and running the project
```
mkdir build && cd build
cmake ..
make
./2D_feature_tracking
```

## Comments, Task MP.0

### MP.1 Data buffer optimization

### MP.2 Keypoint detection

### MP.3 Keypoint removal

### MP.4 Keypoint descriptors

### MP.5 Descriptor matching

### MP.6 Descriptor distance ratio

### MP.7 Performance evaluation 1

### MP.8 Performance evaluation 2

### MP.9 Performance evaluation 3
