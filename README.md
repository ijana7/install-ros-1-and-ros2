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

## ros2
 first write in terminal :

 locale  # to check for UTF-8
 
 <img width="1009" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٨ في ٤ ٥١ ٣٥ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/3d62b176-5833-4a19-9f9d-7212380e1d72">
 
setup sources:
 
sudo apt install software-properties-common

Now add the ROS 2 GPG key with apt.Now add the ROS 2 GPG key with apt:

sudo apt update && sudo apt install curl -y

Then add the repository to your sources list:
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null

install ros 2 packages

sudo apt update

sudo apt upgrade

<img width="999" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٨ في ٤ ٥٢ ٣٢ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/84feb4c3-4f07-4167-a8b4-531c88343205">

Desktop Install (Recommended): ROS, RViz, demos, tutorials:

sudo apt install ros-foxy-desktop python3-argcomplete

<img width="1035" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٨ في ٤ ٥٣ ٣٨ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/069be275-1fc2-45ee-b71f-bda4ee587c17">

enviornment setup :

source /opt/ros/foxy/setup.bash

<img width="1005" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٨ في ٤ ٥٤ ٥٨ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/82bde61a-4986-474d-90d3-11fec976867e">

try some ex :
ros2 run demo_nodes_cpp talker

ros2 run demo_nodes_py listener

<img width="1710" alt="‏لقطة الشاشة ١٤٤٥-١٢-٢٧ في ٩ ٥٠ ٠٩ م" src="https://github.com/ijana7/install-ros1-and-ros2/assets/173642526/7e01c2df-707d-4fb0-931e-da3a403d55a6">
