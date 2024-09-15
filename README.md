# ROS 2 Robot Simulation Project

This project is part of the ROS 2 Mentorship Program at Rigbetel Labs. It demonstrates the integration of a custom-designed robot into Gazebo and RViz2, along with keyboard control and sensor plugins.

## Features

- **CAD to URDF Conversion:** The robot was designed using Fusion 360 or SolidWorks and converted into a URDF package.
- **Custom Robot Description:** Description file customized for both Gazebo and RViz2, including colors.
- **Custom Gazebo World:** Integrated the robot into a custom-built Gazebo world.
- **Robot Control:** Control the robot using the `teleop_twist_keyboard` package for keyboard input.
- **Sensors:** Camera and laser sensor plugins were added to the robot.
- **Visualization:** The robot and sensors were visualized in RViz2.

## Prerequisites

- ROS 2 Humble installed.
- Gazebo and RViz2 set up for ROS 2.

## How to Run the Project

### 1. Build the Package

Run the following command in your ROS 2 workspace to build the package:

```bash
yash@ubuntu22:~/ros_ws$ colcon build
