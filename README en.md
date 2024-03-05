[简体中文](./README.md) | 简体中文

# Feature Introduction

This is a quick start guide for NodeHub, which demonstrates how to control a small turtle for drawing using keyboard commands.

# Material List

The following robots are compatible with RDK X3:

Material Option	List
Robot Name	Manufacturer
RDK X3 Robot	Multiple Manufacturers
# Usage

Preparation
Make sure your RDK X3 is using the desktop version and has stable internet access.
Install the first-node Function Package
After starting the robot, connect to it via a terminal or VNC. Click the "One-Click Deployment" button in the upper right corner, copy the command, and run it on the RDK system to complete the installation of the hobot-nav2 function package.

Bash
sudo apt update
sudo apt install -y tros-first-node
请谨慎使用代码。
Use Keyboard to Control Turtlesim
Connect to the robot using MoBaXterm and start the following commands:

Bash
# Set the tros environment variable
source /opt/tros/setup.bash

# Start Turtlesim
ros2 run turtlesim turtlesim_node
请谨慎使用代码。
In another terminal, start turtle_teleop_key:

Bash
# Set the tros environment variable
source /opt/tros/setup.bash

# Start OriginBot
 ros2 run turtlesim turtle_teleop_key
请谨慎使用代码。
Use the keyboard arrow keys (up, down, left, right) to control the movement of turtlesim.

# Interface Description

Published Topics
Name	Message Type	Description
/turtle1/cmd_vel	geometry_msgs/msg/Twist	turtlesim motion control command
# References

None
# FAQ

None