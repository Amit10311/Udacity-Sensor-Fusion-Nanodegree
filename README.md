# Udacity-Sensor-Fusion-Nanodegree
In this program, I have learned knowledge in different sensors, Lidar, Camera and Radar. Code has been developed to detect obstacles using Lidar point cloud data, to track the object using Camera images, to detect range and velocity of targe based on Radar data, and to fuse Lidar/Radar measurement to predict the object's movement using Kalman Filter.

| Criteria                      | Lidar                                           | Radar                          | Camera                                                                                       |
|-------------------------------|-------------------------------------------------|--------------------------------|----------------------------------------------------------------------------------------------|
| **Range**                      | Meters to 200m                                  | Meters to 200m                 | Only stereo camera setup can measure distance up to 80m                                       |
| **Spatial Resolution**         | High, 0.1 degree due to short wavelength laser  | Cannot resolve small features  | Defined by optics, pixel size of image and its signal-to-noise ratio                          |
| **Robustness in Darkness**     | Excellent, due to active                        | Excellent, due to active       | Reduced                                                                                      |
| **Robustness in Rain, Snow, Fog**| Limited, due to optical                        | Best                           | Limited, due to optical                                                                       |
| **Classification of Objects**  | Some level of classification by 3D point clouds | Not too much classification    | Excellent at classification                                                                  |
| **Perceiving 2D Structures**   | N/A                                             | N/A                            | The only sensor that is able to interpret traffic signs, lane markings, traffic lights        |
| **Measure Speed**              | Approximate speed by using successive distance measurement | Measure velocity by exploiting the Doppler frequency shift | Can only measure time to collision by observing the displacement of objects on the image plane |
| **System Cost**                | More expensive                                  | Compact and affordable         | Compact and affordable                                                                       |
| **Package Size**               | Hard to integrate                               | Easily integrated              | Easily integrated for mono cameras, but stereo camera setup is bulky                         |
| **Computational Requirements** | Little                                          | Little                         | Significant                                                                                  |



Sensor Fusion by combing Lidar's high resolution imaging with radar's ability to measure velocity of objects we can get a better understanding of the surrounding environment than we could using one of the sensors alone.

Project 1 - Lidar Obstacle Detection
In this project, I processed multiple point clouds data files from Lidar sensor, and detected the cars or other obstacles on a city street. The detection pipeline was implemented by the Voxel Grid and ROI based filtering, 3D RANSAC segmentation, Euclidean clustering based on KD-Tree, and bounding boxes.

My final result is shown below, where the green points represent the street surface and the obstacles are marked in the red boxes.


## Lecture Notes
[Lecture 1-1 Lidar and Point Cloud](https://github.com/Amit10311/Udacity-Sensor-Fusion-Nanodegree/blob/main/lectures/lec1_1-lidar-and-point-clouds.md)


### Resources 
1. https://github.com/fanweng/Udacity-Sensor-Fusion-Nanodegree/tree/main
