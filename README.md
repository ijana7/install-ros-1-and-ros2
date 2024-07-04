# install-ros-1-and-ros2
ROS1 is an open-source robotics framework that enables building robotic applications. 

## stepes to dowanload
first you shold Configure your Ubuntu repositories

Setup your sources.list :

sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

Set up your keys :

sudo apt install curl # if you haven't already installed curl

Installation :

sudo apt update

Now pick how much of ROS you would like to install.

Desktop Install: Everything in ROS-Base plus tools like rqt and rviz  :

sudo apt install ros-noetic-desktop

sudo apt install ros-noetic-PACKAGE 

sudo apt install ros-noetic-slam-gmapping

To find available packages:

apt search ros-noetic

Environment setup:

source /opt/ros/noetic/setup.bash

echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.zshrc

Dependencies for building packages :

sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential

Initialize rosdep :

sudo apt install python3-rosdep

you can initialize rosdep :

sudo rosdep init
rosdep update
