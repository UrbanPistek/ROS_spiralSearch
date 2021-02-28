# Project Details
## Summary
Developed a custom ROS package with custom launch files, services, actions and messages to implement a Spiral Search Algorithm as a 
ROS Action Server. The Spiral Search Alogirthm was tested using the turtlesim node with an action client running on Ubuntu 18.04 VM with 
ROS Melodic.

## Setting the Workspace
    $ mkdir -p ~/catkin_ws/src
    $ cd ~/catkin_ws/
    $ catkin_make
    $ source devel/setup.bash
Add the spiral search package to the workspace `src/` directory. 

### Build the Node
    ~/catkin_ws$ catkin_make
    ~/catkin_ws$ source devel/setup.bash

## Run the Node
#### Run roscore
    ~/catkin_ws$ roscore

#### Run the action server
    ~/catkin_ws$ rosrun spiralSearch spiralSearch_server

#### In a new terminal run turtlesim
    ~$ rosrun turtlesim turtlesim_node

#### Run the action client
    ~/catkin_ws$ rosrun spiralSearch spiralSearch_server 