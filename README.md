Notes for ROS
=============

## ROS communication

* nodes
* topics
* messages

## ROS tools

* rqt_graph -> To see node and topic configuration
* rqt_plot -> To plot some messages data
* rqt_reconfigure -> Reconfigure some parameters of nodes
* rosbag -> Keep track of all the sensor data
* rviz -> Augmented reality tool
* RQt -> ROS GUI

## Practise

Always check the environment variable before to start.

### ROS package management

* `rospack` -> information about the ROS package
* `roscd` -> command to navigate in the package directory
* `rosmsg` -> information about the messages information
* `rosbag` -> to handle the bag file

You need to start ROS using `roscore`.

#### `rosbag`

* To play a bag -> `rosbag play file.bag`
* To record a bag -> `rosbag record -o file.bag`

#### `rostopics`

* To list the topics -> `rostopics list`
* To echo the topics -> `rostopics echo /topic`

You can start by listing to know if you are publishing any messages.

#### `rosnodes`

* To list the nodes -> `rosnode list`
* To kill node -> `rosnode kill /node`

#### Time management

We need to force the simulation time when dealing with bag.
There is a topic called `/clock` topic.

* Set the time at simulation: `rosparam set use_sim_time true`
* Get the time: `rosparam get use_sim_time`

#### `rviz`

* Setup the fixed frame to `odom`
* Add other message topics

