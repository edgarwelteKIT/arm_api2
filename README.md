# arm_api2

API for the robotic manipulators realying on: 
* [Moveit2](https://moveit.picknik.ai/main/index.html)
* [ROS 2](https://docs.ros.org/en/humble/index.html)

Docker for building required environment can be found [here](https://github.com/larics/docker_files/tree/master/ros2-humble/moveit2). 

For building ROS 2 packages and moveit, it is neccessary to use [colcon](https://colcon.readthedocs.io/en/released/user/quick-start.html). 

#### Build just one package: 

```
colcon build --packages-select arm_api2
```

## Aim of the repository

With `arm_api` as precursor, which was intended to provide simple ROS interfacing with 
robot manipulators with the help of moveit. 

This repository `arm_api2` is intended to provide interfacing support for robot manipulators for ROS 2 and MoveIt2!. 

## Goals 

Create API simple to **run** and **maintain** that supports working with different 
robot manipulators out of the box. 

Robot manipulators of interest are: 
* Franka Emika
* UR 
* Kinova 
* Kuka 

Wanted arm functionalities: 
1. `go_to_pose`
2. `grasp` 


## Status: 

### DONE: 
- [x] Create pkg skeleton 
- [x] Build moveit2 and ros 2 Docker 

### TODO: 
- [ ] Go through moveit2 tutorials 
- [ ] Define SW patterns that makes sense to use





