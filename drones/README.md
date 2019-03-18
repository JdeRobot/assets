Unmaned Aerial Vehicles in JdeRobot with ROS
========

The new Hardware Abstraction Layer (HAL) for working in robotic applications for Unmanned Aerial Vehicles (UAVs) in JdeRobot is based on using ROS/Gazebo and:

* [PX4](https://px4.io/) as main flight control software. 
* [MavROS](http://wiki.ros.org/mavros) as MAVLink-based communication node between ROS and the PX4 flight stack. It also provides an UDP bridge for MAVLink Ground Control Stations

# Installation instructions

You can use [this bash script](https://raw.githubusercontent.com/PX4/Devguide/master/build_scripts/ubuntu_sim_ros_gazebo.sh) for from [dev.px4.io](https://dev.px4.io/en/setup/dev_env_linux.html#gazebo-with-ros) for setting up ROS Kinetic/Gazebo + PX4 + MavROS on Ubuntu 16.04 (Xenial). It also installs some common dependencies libraries and tools 

Alternatively, it can be done step by step:

## ROS Kinetic and Gazebo 7

ROS must be installed first. Please follow [the official instructions](http://wiki.ros.org/kinetic/Installation/Ubuntu) to install ROS Kinetic (that includes Gazebo 7 by default) in Ubuntu 16.04 (Xenial)

## MavROS

Install MavROS package and its required dependencies following [these installation instructions](https://github.com/mavlink/mavros/blob/master/mavros/README.md#installation). Binary installation (deb packages) is recommended.

## PX4 SITL

Detailed instructions about the PX4 toolchain installation can be found [here](). In summary, you must first:
* Remove the [Ubuntu modemmanager](https://dev.px4.io/en/setup/dev_env_linux_ubuntu.html#remove-the-modemmanager)
* Install the [Common Dependencies](https://dev.px4.io/en/setup/dev_env_linux_ubuntu.html#common-dependencies)
* Install the [Ninja Build System](https://dev.px4.io/en/setup/dev_env_linux_ubuntu.html#ninja-build-system)
* Install [FastRTPS](https://dev.px4.io/en/setup/dev_env_linux_ubuntu.html#fastrtps-installation)

After that, download the last PX4 Firmware from its Github repository:

```sh
git clone https://github.com/PX4/Firmware.git 
```

Build the PX4 stack for SITL in Gazebo. You can find more info about building PX4 for different boards, models and variants [here](https://dev.px4.io/en/setup/building_px4.html#make_targets). 

```sh
cd <Firmware>
make px4_sitl_default gazebo
source Tools/setup_gazebo.bash $(pwd) $(pwd)/build/px4_sitl_default
export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:$(pwd)
export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:$(pwd)/Tools/sitl_gazebo
```

## PX4 SITL + MavROS launch files

A default launch file for launching PX4 SITL + MavROS + Gazebo is included in the MavROS package: 

```sh
roslaunch px4 mavros_posix_sitl.launch 
```
It will load the default 3DR Iris model in Gazebo:

![3DR Iris](/images/3DR_Iris.jpg?raw=true)


For launching the 3DR Solo model, use:

```sh
roslaunch px4 mavros_posix_sitl.launch vehicle:=solo 
```

![3DR Solo](/images/3DR_Solo.jpg?raw=true)

## Adding a front camera to the simulated model

If you need to simulate a quadcopter with front RGB camera, you can launch the iris_fpv_cam model 

```sh
roslaunch px4 mavros_posix_sitl.launch vehicle:=iris_fpv_cam
```

![3DR Iris FPV Cam](/images/3DR_Iris_fpvcam.jpg?raw=true)

*Note: Sometimes there are problems with launching the former vehicle, and Gazebo crashes. It needs to be checked.
For those cases, there is already a solution that would be addressed here in the near future.* 

## Hardware compatibility

This HAL is compatible with any UAVs including a Pixhawk flight controller or any other board flashed with the PX4 stack. 

* A list of compatible boards can be found [here](https://docs.px4.io/en/flight_controller/#documented-boards)
* Some complete UAVs run PX4 "out of the box". There is a list [here](https://docs.px4.io/en/complete_vehicles/) 
