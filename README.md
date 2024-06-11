# TurtleBot2 ROS 2 Description

This repository provides the ROS 2 description for TurtleBot2 with Hokuyo and Kinect sensors. You can visualize the robot in RViz using the provided launch files.

## Features

- **Reference:** Edited based on [TurtleBot2 Description](https://github.com/igrak34/turtlebot2-ros2/tree/humble-devel/turtlebot2_description)
- **Customizable Sensor Positions:** The positions of the Hokuyo and Kinect sensors can be adjusted to match your robot's configuration.
- **Prefix Specification:** The prefix for the robot can be freely specified. By default, it is set to `turtlebot/`.

## Usage

### Launching the Robot Description

To display the TurtleBot2 in RViz with the specified sensor configuration:

```
ros2 launch turtlebot2_description display_with_kinect_hokuyo.launch.py
```

### Changing the prefix
By default, the robot's prefix is set to turtlebot/. To change it, edit the prefix declaration in the robots/kobuki_hexagons_kinect_hokuyo.xacro file:
```
<xacro:property name="prefix" value="your_custom_prefix"/>
```
