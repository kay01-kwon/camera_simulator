# camera_simulator
RealSense D435 camera in Gazebo

Environment: Ubuntu 20.04 Noetic

Prerequisite

1. Install realsense2_description pkg

$ sudo apt-get install ros-noetic-realsense2-description

2. Go to the site https://github.com/pal-robotics/realsense_gazebo_plugin

and clone this package into the ~/catkin_ws/src directory.

Then, build it.

3. Get this package and then launch it.

$ roslaunch camera_simulator realsense2_gazebo.launch

More Info.

Replace <pointCloud>false</pointCloud> with <pointCloud>true</pointCloud> to get point cloud data.

<img src="/camera_simulator/reference/XML.png" width="500" height="400" />

Implementation in Gazebo version 11

<img src="/camera_simulator/reference/Gazebo_Realsense_Camera.png" width="500" height="400" />

RVIZ point cloud data

<img src="/camera_simulator/reference/pointcloud_data_in_RVIZ.png" width="500" height="400" />
