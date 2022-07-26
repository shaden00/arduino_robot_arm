# arduino_robot_arm
In this task we will use some of Ros packages to see how we could move the robot arm , and we can do it in simulation and real-life, i tested these packages under ros noetic and ubuntu 20.04

ارجع اكتب السميوليشن و الموف و الجوينت

# Dependencies
* fist we need to run this instruction 
`$ rosdep install --from-paths src --ignore-src -r -y` 

* second i installed noetic distro package by run these instructions 
```
$ sudo apt-get install ros-noetic-moveit
$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
```
