# Task2-SM-
Installing and operating the arm package on the ros system
# Installing Ros:

1-Download VirtualBox

‎‏ VirtualBox download link:

‎‏ https://www.virtualbox.org/wiki/Downloads

‎2-‏ Download ubuntu20.04

‎‏ ubuntu20.04 download link:

‎‏ https://releases.ubuntu.com/20.04/


‎‏3-How to install Ros1

‎‏ Run Terminal and type the following commands:

‎‏ Command Prompt Link:

‎‏ http://wiki.ros.org/Installation/Ubuntu

# Installing and operating the arm package on the ros system: 

Command Prompt Link::

https://s-m.com.sa/ros.txt

$ cd ~/catkin_ws/src

$ sudo apt install git

$ git clone https://github.com/smart-methods/arduino_robot_arm

Install all the dependencies :

$ cd ~/catkin_ws

$ rosdep install --from-paths src --ignore-src -r -y

For noetic:

$ sudo apt-get install ros-noetic-moveit

$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui

$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher

$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line

(source /home/nawal/catkin_ws/devel/setup.bash)

then (ctrl + o , enter, ctel+x)

source ~/.bashrc

roslaunch robot_arm_pkg check_motors.launch

Compile the package:

$ catkin_make

moveit:

$ roslaunch moveit_pkg demo.launch
