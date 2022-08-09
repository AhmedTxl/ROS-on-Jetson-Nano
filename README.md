## Installing ROS on Jetson Nano

This is a required task that is about how to install ROS on Jetson Nano

The Robot Operating System (ROS) is a set of software libraries and tools that help you build robot applications. From drivers to state-of-the-art algorithms, and with powerful developer tools, ROS has what you need for your next robotics project. And it's all open source.<br>
[![ROS Melodic](http://www.ros.org/news/2018/04/16/melodic_logo.jpg "ROS Melodic")](http://www.ros.org/news/2018/04/16/melodic_logo.jpg "ROS Melodic")

Jetson Nano is a small, powerful computer for embedded applications and AI IoT that delivers the power of modern AI
[![Jetson Nano](https://developer.nvidia.com/sites/default/files/akamai/embedded/images/jetsonNano/nvidia-jetson-nano-module-standing-2c50-d.jpg "Jetson Nano")](https://developer.nvidia.com/sites/default/files/akamai/embedded/images/jetsonNano/nvidia-jetson-nano-module-standing-2c50-d.jpg "Jetson Nano")

## Requirements Before Start:
- Ubuntu Operating System (Very Recommended Version 18)

## Installing Guide: 
- Open a new terminal by pressing Ctrl + Alt + t or executing the “Terminal” application using the Ubuntu 18 launch system.
- Then setup Jetson Nano to accept ROS packages and the apt-key by using these command:
	- $ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu
	- $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
	- $ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
- After that we need to update the Debian packages index by this command:
	- $ sudo apt update
- Now we will install the ROS Melodic by this command (Recommended to install the FULL Version of ROS Melodic):
	- $ sudo apt install ros-melodic-desktop
- A recommended step which is load the ROS environment varibales automatically when executes a new shell by this two commands: 
	- $ echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc 
	- $ source ~/.bashrc
- Now we will install rosdep, rosdep enables the user to easily instal system dependencies for source code you want to compile and is required to run some core components in ROS, and these are the commands for this step:
	- $ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
	- $ sudo rosdep init 
	- $ rosdep update
- Now the Jetson Nano is ready to execute ROS to packages to start your journey in making robots :tw-1f496:

## Refrences
- https://www.stereolabs.com/blog/ros-and-nvidia-jetson-nano/
- https://developer.nvidia.com/embedded/jetson-nano-developer-kit

## This work has been done by: Ahmed Wasel Alharbi

