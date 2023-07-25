# ROS/ROS2 bridge for CARLA simulator 0.9.14 with a Livox lidar

This is fork of an official CARLA-ROS bridge 0.9.13 with [Livox lidar sensor created by IKAROS93](https://github.com/IKAROS93/Livox_laser_simulation_for_CARLA).

The files from [the official repository *(commit #630)*](https://github.com/carla-simulator/ros-bridge/commit/e9063d97ff5a724f76adbb1b852dc71da1dcfeec) were merged with files created by IKAROS93 and desired version of CARLA was changed to prevent errors.

New launchgile **carla_example_ego_vehicle_with_livox.launch.py** was added to spawn an ego vehicle with Livox lidar attached.

*And pull request fixing HUD info about cardinal direction in **CARLA Manual Control** package were merged*.



# ROS/ROS2 bridge for CARLA simulator

[![Actions Status](https://github.com/carla-simulator/ros-bridge/workflows/CI/badge.svg)](https://github.com/carla-simulator/ros-bridge)
[![Documentation](https://readthedocs.org/projects/carla/badge/?version=latest)](http://carla.readthedocs.io)
[![GitHub](https://img.shields.io/github/license/carla-simulator/ros-bridge)](https://github.com/carla-simulator/ros-bridge/blob/master/LICENSE)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/carla-simulator/ros-bridge)](https://github.com/carla-simulator/ros-bridge/releases/latest)

 This ROS package is a bridge that enables two-way communication between ROS and CARLA. The information from the CARLA server is translated to ROS topics. In the same way, the messages sent between nodes in ROS get translated to commands to be applied in CARLA.

![rviz setup](./docs/images/ad_demo.png "AD Demo")

**This version requires CARLA 0.9.13**

## Features

- Provide Sensor Data (Lidar, Semantic lidar, Cameras (depth, segmentation, rgb, dvs), GNSS, Radar, IMU)
- Provide Object Data (Transforms (via [tf](http://wiki.ros.org/tf)), Traffic light status, Visualization markers, Collision, Lane invasion)
- Control AD Agents (Steer/Throttle/Brake)
- Control CARLA (Play/pause simulation, Set simulation parameters)

## Getting started and documentation

Installation instructions and further documentation of the ROS bridge and additional packages are found [__here__](https://carla.readthedocs.io/projects/ros-bridge/en/latest/).
