Tutorial ROS #2 - Lecture notes
===============================

# Introduction to start navigate the robot

* Connect via ssh: `ssh turtlebot@192.168.0.100`
* Start minimal launch: `roslaunch kokubi_node minimal.launch --screen`
* Start with `tf` topic: `roslaunch kobuki_node robot_with_tf.launch --screen`
* Launch the following node to manage the robot with keyboard: `roslaunch kobuki_keyop keyop.launch`

# Move to the turtlebot launcher

* Start the minimal launcher: `roslaunch turtlebot_bringup minimal.launch`
* Install the `turtlebot` packages for the turtlebot via the package manager: `sudo apt-get install ros-indigo-turtlebot-*`
* Launch the kinect: `roslaunch turtlebot_bringup 3dsensor.launch`

