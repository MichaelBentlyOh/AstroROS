# AstroROS
Spacecraft Orbit/Attitude Simulation
# Introduction
This repository is for AstroROS : ADR simulator for On-Orbit Servicing.

This repo is a fork repo from https://github.com/uscl/AstroROS .

Every changes (even they are trivial) will be applied in this repo and revised version will be uploaded in original repository.
# How to use AstroROS
1. Install ROS noetic(ubuntu 20.04)
2. Clone "reaction_wheel_tentacle_ws" (do not care about "orbit_simulator_matlab")
```
git clone https://github.com/MichaelBentlyOh/AstroROS.git
```
3. Get into "reaction_wheel_tentacle_ws" and build workspace
```
cd reaction_wheel_tentacle_ws && catkin build
```
4. Source "setup.bash" in workspace
```
source devel/setup.bash
```
5. Launch the project
```
roslaunch reaction_wheel_main gazebo.launch
```
Then, gazebo will open and there are two objects in gazebo world.

6. give command topics to tentacle satellite.
For demo, I use "rqt".

(2024.07.02) This repository doesn't have tentacle command publisher. After update, command publisher will be added in this repo.

# Update Log
2024.07.01 : fork from https://github.com/uscl/AstroROS

2024.07.02 : update readme.md
# Update plan
<1> Implementation of orbit simulator in C++ with Eigen library(2024.10.31)

<2> Migration from ROS1 to ROS2(2024.12.31)

<3> Application into SpaceROS(https://github.com/space-ros) (2025.??.??)
