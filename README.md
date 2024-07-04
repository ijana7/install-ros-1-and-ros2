# install-ros-1-and-ros2
ROS1 is an open-source robotics framework that enables building robotic applications. 

## stepes to dowanload
first you shold Configure your Ubuntu repositories

Setup your sources.list :

sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

<img width="1194" alt="1" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/7d4d3047-7626-41e0-b83f-e2074f0bf222">

Set up your keys :

sudo apt install curl 


<img width="951" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٨ في ٤ ٣٦ ٠٥ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/9b152bc7-4d6c-4c4e-8af6-cf0a166aae70">

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

<img width="1005" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٨ في ٤ ٣٧ ٥٠ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/962798d6-2cee-4cb0-9d6c-28e210547089">

you can initialize rosdep :

sudo rosdep init
rosdep update
## ran rviz 
<img width="1003" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٨ في ٤ ٤٠ ١٤ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/7e893622-8d81-4840-a573-bda47bbef488">
