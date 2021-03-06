# **Camera Pose Estimation**
Given a map contians street-view images and 3D data (e.g. lidar, SfM point cloud, or depth), estimate the 6 DoF camera pose of a query image.

* **Input of the system**: query image, reference image and lidar point cloud, where reference image and lidar are known in a global coordinate system.

* **Output of the system**: 6 DoF camera pose of the query image in the global coordinate system.

Note: _6 DoF camera pose_ mean _3 DoF translation_ and  _3 DoF rotation_ along _x_, _y_, _z_ axis. 

### One example of query and reference images
![][image0]

### System outputs
![][image1]

## Code & Files
### 1. Dependencies & environment

* Matlab 2016b
* OS: Ubuntu 16.04 (should work on other platform too)

### 2. My project files

(Note: the hyperlinks **only** works if you are on the homepage of this GitHub reop,
and if you are viewing it in "github.io" you can be redirected by clicking the **View the Project on GitHub** on the top)

* [main.m](main.m) is the main code for this demo.

* [read_pose.m](read_pose.m) read camera pose.

* [read_lidar_binary.m](read_lidar_binary.m) read lidar bianry file.

* [ref.m](ref.m) is the class of reference image.

* [world2Image.m](world2Image.m) is the function of project points from world to image.

* [test](data) folder contains the test data.

* [source](source) folder contains the example images.

### 3. How to run the code

(1) Install Matlab (tested with 2016b and 2017a).

(2) Set your current path to this demo and run `main.m`.


## Release History

* 0.1.1
    * Update visualization code and font size
    * Date 24 April 2017

* 0.1.0
    * The first proper release
    * Date 22 April 2017


[//]: # (References)
[image0]: source/images.jpg
[image1]: source/objects.jpg


