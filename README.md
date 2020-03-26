# assets

This repository contains all models and worlds required by the JdeRobot exercises. An effort has been made to have minimal new models and reuse the official models as much as possible. This is due to the fact that any models that are available through the official sources and are not available in the system are automatically downloaded and saved for future usage (This does mean that the first time boot may be much slower - depending on one's internet connection)

The `kinetic-devel` branch has been released on the official ROS build farm and can be downloaded using the command:

## Installation

### ROS Kinetic

```bash
sudo apt-get install ros-kinetic-jderobot-assets
```

### ROS Melodic

```bash
sudo apt-get install ros-melodic-jderobot-assets
```


## ROS Distro Support

|         | Kinetic | Melodic |
|:-------:|:-------:|:-------:|
| Branch  | [`kinetic-devel`](https://github.com/JdeRobot/assets/tree/kinetic-devel) |[`master`](https://github.com/JdeRobot/assets/tree/master)|
| Status  |  supported | supported |
| Version | [version](http://repositories.ros.org/status_page/ros_kinetic_default.html?q=jderobot_assets) |[version](http://repositories.ros.org/status_page/ros_melodic_default.html?q=jderobot_assets)|

## ROS Buildfarm

|         |  Kinetic Source  |  Kinetic Debian |  Melodic Source  |  Melodic Debian |
|:-------:|:-------------------:|:-------------------:|:-------------------:|:-------------------:|
| jderobot_assets | [![released](http://build.ros.org/buildStatus/icon?job=Ksrc_uX__jderobot_assets__ubuntu_xenial__source)](http://build.ros.org/view/Ksrc_uX/job/Ksrc_uX__jderobot_assets__ubuntu_xenial__source/) | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uX64__jderobot_assets__ubuntu_xenial_amd64__binary)](http://build.ros.org/view/Kbin_uX64/job/Kbin_uX64__jderobot_assets__ubuntu_xenial_amd64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Msrc_uB__jderobot_assets__ubuntu_bionic__source)](http://build.ros.org/view/Msrc_uB/job/Msrc_uB__jderobot_assets__ubuntu_bionic__source/) | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_uB64__jderobot_assets__ubuntu_bionic_amd64__binary)](http://build.ros.org/view/Mbin_uB64/job/Mbin_uB64__jderobot_assets__ubuntu_bionic_amd64__binary/)