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

