# TurtleBot3 Setup Guide

## Initial Setup

In one terminal after cloning and entering the repo do the following:

```bash
rm -rf ~/.build ~/.log ~/.install
colcon build
source install/setup.bash
ros2 launch turtlebot3_gazebo turtlebot3_world.launch.py
```

This will launch the custom designed urdf of the differential drive robot in a custom world created from scratch.

## Navigation Setup

Next open another terminal and copy paste the following commands:

```bash
source install/setup.bash
export TURTLEBOT3_MODEL=burger
ros2 launch turtlebot3_navigation2 navigation2_use_sim_time.launch.py
```
