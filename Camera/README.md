# Camera Projects

This repo contains lesson-wise exercises and corresponding solutions for Udacity's Sensor Fusion ND.

## I. List of Lesson-wise Exercises
* Original source code of lesson exercises is available here - https://github.com/udacity/SFND_Camera
 
  * Lesson 2: Autonomous Vehicles and Computer Vision [(Lecture/Exercise notes :TODO)]()
    * The OpenCV Library
  * Lesson 3: Engineering a Collision Detection System [(Lecture/Exercise notes :TODO)]()
    * Estimating TTC with Camera
    * Estimating TTC with Lidar
  * Lesson 4: Tracking Image Features [(Lecture/Exercise notes :TODO)]()
    * Descriptor Matching
    * Gradient-based vs. Binary Descriptors
    * Harris Corner Detection
    * Intensity Gradient and Filtering
    * Overview of Popular Keypoint Detectors
  * Lesson 6: Combining Camera and Lidar [(Lecture/Exercise notes :TODO)]()
    * Creating 3D-Objects
    * Lidar-to-Camera Point Projection
    * Object Detection with YOLO
  * Projects
    * Lesson 5: Starter code for "Project: Camera Based 2D Feature Tracking" is available here - https://github.com/udacity/SFND_2D_Feature_Tracking
      * Project report (HERE)
    * Lesson 7: Starter code for "Project: Track an Object in 3D Space" is available here - https://github.com/udacity/SFND_3D_Object_Tracking
      * Project report (HERE)

### II. Dependencies for Running Locally
1. cmake >= 2.8
   * All OSes: [click here for installation instructions](https://cmake.org/resources/)

2. make >= 4.1 (Linux, Mac), 3.81 (Windows)
   * Linux: make is installed by default on most Linux distros
   * Mac: install Xcode command line tools to get make
   * Windows: Click here for installation instructions

3. OpenCV >= 4.1
   * This must be compiled from source using the `-D OPENCV_ENABLE_NONFREE=ON` cmake flag for testing the SIFT and SURF detectors.
   * The OpenCV 4.1.0 source code can be found [here](https://github.com/opencv/opencv/tree/4.1.0)
   * Install the OpenCV dependencies as well as OpenCV Contrib for extra modules, then build from the source. Instruction [HERE](http://techawarey.com/programming/install-opencv-c-c-in-ubuntu-18-04-lts-step-by-step-guide/).
   * **NOTE:** the license issue still might occur when using non-free algorithms, in that case, please use the online workspace provided by Udacity.
```
# compiler
$ sudo apt-get install build-essential
# required
$ sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev libcanberra-gtk-module
# optional
$ sudo apt-get install python-dev python-numpy libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev libdc1394-22-dev

$ git clone https://github.com/opencv/opencv.git
$ git clone https://github.com/opencv/opencv_contrib.git <opencv_contrib_dir>
$ cd ./opencv
$ mkdir build && cd build
$ cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/usr/local -DOPENCV_EXTRA_MODULES_PATH=<opencv_contrib_dir>/modules -DOPENCV_ENABLE_NONFREE=ON ..
$ make -j4
$ sudo make install
```
4. gcc/g++ >= 5.4
   * Linux: gcc / g++ is installed by default on most Linux distros
   * Windows: recommend using MinGW

### III. Build Instructions
Go to the top level directory for an exercise or a project where the `CMakeLists.txt` file locates, and run the following commands on the Linux terminal:
```
$ mkdir build && cd build
$ cmake ..
$ make
$ ./<Executable_File_Name>
```
