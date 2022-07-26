# arduino_robot_arm
In this task we will use some of Ros packages to see how we could move the robot arm , and we can do it in simulation and real-life, i tested these packages under ros noetic and ubuntu 20.04

ارجع اكتب السميوليشن و الموف و الجوينت

# Dependencies
* first we need to run this instruction 
`$ rosdep install --from-paths src --ignore-src -r -y` 

* second i installed noetic distro package by run these instructions 
```
$ sudo apt-get install ros-noetic-moveit
$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
```

# Configuring Arduino with ROS
so here we will Configur Arduino with ROS by these steps
1. install Arduino IDE in Ubuntu from [HERE](https://www.arduino.cc/en/software)
* extraxt the folder
* open the terminal inside the folder
* run the instruction `$ sudo ./install.sh ` 
* now open the Arduino IDE to make sure that it installed successfully
2. Install the arduino package , by Installing Binaries on the ROS workstation
* run these instructions
```
sudo apt-get install ros-noetic-rosserial-arduino
sudo apt-get install ros-noetic-rosserial
```
3. install ros library into the Arduino Environment , The preceding installation steps created the necessary libraries, now the following will create the ros_lib folder that the Arduino build environment needs to enable Arduino programs to interact with ROS
```
cd <sketchbook>/libraries
rm -rf ros_lib
rosrun rosserial_arduino make_libraries.py .

```
**(sketchbook) is the directory where the Linux Arduino environment saves your sketches. Typically this is a directory called sketchbook or Arduino in your home directory. e.g cd ~/Arduino/libraries**

4. so if you open the Arduino IDE , you should see ros_lib listed under examples

![image](https://user-images.githubusercontent.com/97844314/181125928-cd3a934d-3f97-4c4f-b71c-3e0718c127af.png)

