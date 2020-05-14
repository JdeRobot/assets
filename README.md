# assets

This repository contains all models and worlds required by the JdeRobot exercises. An effort has been made to have minimal new models and reuse the official models as much as possible. This is due to the fact that any models that are available through the official sources and are not available in the system are automatically downloaded and saved for future usage (This does mean that the first time boot may be much slower - depending on one's internet connection)

## Installation

### ROS Melodic 

The `master` branch has been released on the official ROS build farm and can be installed using the command:

```bash
sudo apt-get install ros-melodic-jderobot-assets
```

### ROS Kinetic

The `master` branch has also been released for ROS Kinetic, however it has reached it's End Of Life (EOL). It can still be installed using the command:

```bash
sudo apt-get install ros-kinetic-jderobot-assets
```

## ROS Distro Support

|         | Melodic | Kinetic |
|:-------:|:-------:|:-------:|
| Branch  | [`master`](https://github.com/JdeRobot/assets/tree/master)| [`master`](https://github.com/JdeRobot/assets/tree/master) |
| Status  | supported | EOL |
| Version | [version](http://repositories.ros.org/status_page/ros_melodic_default.html?q=jderobot_assets)| [version](http://repositories.ros.org/status_page/ros_kinetic_default.html?q=jderobot_assets) |

## ROS Buildfarm

### Ubuntu

|         |  Melodic Bionic |  Kinetic Xenial  |
|:-------:|:-------------------:|:-------------------:|
| source | [![released](http://build.ros.org/buildStatus/icon?job=Msrc_uB__jderobot_assets__ubuntu_bionic__source)](http://build.ros.org/job/Msrc_uB__jderobot_assets__ubuntu_bionic__source/) | [![released](http://build.ros.org/buildStatus/icon?job=Ksrc_uX__jderobot_assets__ubuntu_xenial__source)](http://build.ros.org/job/Ksrc_uX__jderobot_assets__ubuntu_xenial__source/)| 
| bin amd64 |[![released](http://build.ros.org/buildStatus/icon?job=Mbin_uB64__jderobot_assets__ubuntu_bionic_amd64__binary)](http://build.ros.org/job/Mbin_uB64__jderobot_assets__ubuntu_bionic_amd64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uX64__jderobot_assets__ubuntu_xenial_amd64__binary)](http://build.ros.org/job/Kbin_uX64__jderobot_assets__ubuntu_xenial_amd64__binary/)| 
| bin i386 | n/a| [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uX32__jderobot_assets__ubuntu_xenial_i386__binary)](http://build.ros.org/job/Kbin_uX32__jderobot_assets__ubuntu_xenial_i386__binary/)| 
| dev amd64 | [![released](http://build.ros.org/buildStatus/icon?job=Mdev__jderobot_assets__ubuntu_bionic_amd64)](http://build.ros.org/job/Mdev__jderobot_assets__ubuntu_bionic_amd64/)| [![released](http://build.ros.org/buildStatus/icon?job=Kdev__jderobot_assets__ubuntu_xenial_amd64)](http://build.ros.org/job/Kdev__jderobot_assets__ubuntu_xenial_amd64/)|
| bin arm64 | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_ubv8_uBv8__jderobot_assets__ubuntu_bionic_arm64__binary)](http://build.ros.org/job/Mbin_ubv8_uBv8__jderobot_assets__ubuntu_bionic_arm64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uxv8_uXv8__jderobot_assets__ubuntu_xenial_arm64__binary)](http://build.ros.org/job/Kbin_uxv8_uXv8__jderobot_assets__ubuntu_xenial_arm64__binary/) |
| bin armhf | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_ubhf_uBhf__jderobot_assets__ubuntu_bionic_armhf__binary)](http://build.ros.org/job/Mbin_ubhf_uBhf__jderobot_assets__ubuntu_bionic_armhf__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uxhf_uXhf__jderobot_assets__ubuntu_xenial_armhf__binary)](http://build.ros.org/job/Kbin_uxhf_uXhf__jderobot_assets__ubuntu_xenial_armhf__binary/) |


### Debian

|         |  Melodic Stretch   | 
|:-------:|:-------------------:|
| source | [![released](http://build.ros.org/buildStatus/icon?job=Msrc_dS__jderobot_assets__debian_stretch__source)](http://build.ros.org/job/Msrc_dS__jderobot_assets__debian_stretch__source/) | 
| bin amd64 | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_ds_dS64__jderobot_assets__debian_stretch_amd64__binary)](http://build.ros.org/job/Mbin_ds_dS64__jderobot_assets__debian_stretch_amd64__binary/) | 
| bin arm64 | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_dsv8_dSv8__jderobot_assets__debian_stretch_arm64__binary)](http://build.ros.org/job/Mbin_dsv8_dSv8__jderobot_assets__debian_stretch_arm64__binary/) | 
