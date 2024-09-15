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
```

### 2. Source the Setup

Source the setup file in all terminals before launching any nodes.

```bash
yash@ubuntu22:~/ros_ws$ source install/setup.bash
```

### 3. Launch Gazebo with the Robot

Launch the robot in the custom Gazebo world

```bash
yash@ubuntu22:~/ros_ws$ ros2 launch ros2_bot_description gazebo.launch.py
```

### 4. Launch the Robot State Publisher

This node publishes the robot’s joint states

```bash
yash@ubuntu22:~/ros_ws$ ros2 launch ros2_bot_description state_publisher.launch.py
```

### 5. Open RViz2 for Visualization

Launch RViz2 for robot and sensor visualization

```bash
yash@ubuntu22:~/ros_ws$ rviz2
```

### 6. Control the Robot with Keyboard

Use the keyboard to control the robot’s movement

```bash
yash@ubuntu22:~/ros_ws$ ros2 run teleop_twist_keyboard teleop_twist_keyboard
```


## Screenshots
### CAD Model in Fusion360
![WhatsApp Image 2024-08-29 at 15 23 44_a7aa8fe3](https://github.com/user-attachments/assets/d7147afd-d434-49de-b0be-ad6325d69430)

## Gazebo Simulation
![Screenshot from 2024-09-15 17-46-48](https://github.com/user-attachments/assets/bab2eb9f-2cc8-4403-8635-986de3d3b174)

## Robot in Custom Gazebo World
![Screenshot from 2024-09-15 17-47-32](https://github.com/user-attachments/assets/8027f039-0de1-4a3f-981c-cf57dd01e093)

## RViz2 Visualization
![Screenshot from 2024-09-15 17-49-34](https://github.com/user-attachments/assets/f7907afd-4765-4a4c-b1b2-c9298c8ab3dc)

## RQT Graph
![Screenshot from 2024-09-15 18-08-50](https://github.com/user-attachments/assets/65273e33-b0a5-4bd7-9a14-8f129826e21b)
