# camera_simulator
RealSense D435 camera in Gazebo

Environment: Ubuntu 20.04 Noetic

Prerequisite

# 1. Install realsense2_description pkg

$ sudo apt-get install ros-noetic-realsense2-description

Before executing catkin_make, check the version of protoc.

How to figure out the version.

$ protoc --version
libprotoc 3.6.1

# Installation of the protoc 3.6.1 IF YOU DO NOT HAVE PROTOBUF 3.6.1

If you do not have protoc version 3.6.1, remove the protoc and then install protoc 3.6.1.

$ mkdir ~/repos && cd ~/repos

~/repos $ wget https://github.com/protocolbuffers/protobuf/releases/download/v3.6.1/protobuf-all-3.6.1.tar.gz

~/repos $ tar -xvzf protobuf-all-3.6.1.tar.gz && cd protobuf-3.6.1

~/repos/protobuf-3.6.1/ $ ./configure

~/repos/protobuf-3.6.1/ $ make

~/repos/protobuf-3.6.1/ $ make check

~/repos/protobuf-3.6.1/ $ sudo make install

~/repos/protobuf-3.6.1/ $ sudo ldconfig

# 2. Go to the site https://github.com/pal-robotics/realsense_gazebo_plugin

and clone this package into the ~/catkin_ws/src directory.

Then, build it.

# 3. Get this package and then launch it.

$ roslaunch camera_simulator realsense2_gazebo.launch

More Info.

Package Contents: 3 urdf files and 1 launch file


<img src="/camera_simulator/reference/contents.png" width="500" height="400" />

Replace <pointCloud>false</pointCloud> with <pointCloud>true</pointCloud> to get point cloud data. (Line 21)

<img src="/camera_simulator/reference/XML.png" width="500" height="400" />

Implementation in Gazebo version 11

<img src="/camera_simulator/reference/Gazebo_Realsense_Camera.png" width="500" height="400" />

RVIZ point cloud data

<img src="/camera_simulator/reference/pointcloud_data_in_RVIZ.png" width="500" height="400" />
