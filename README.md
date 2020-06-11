# assets

This repository contains all models and worlds required by the JdeRobot exercises. An effort has been made to have minimal new models and reuse the official models as much as possible. This is due to the fact that any models that are available through the official sources and are not available in the system are automatically downloaded and saved for future usage (This does mean that the first time boot may be much slower - depending on one's internet connection)

## Installation

### ROS Noetic

The `noetic-devel` branch has been released on the official ROS build farm and can be installed using the command:

```bash
sudo apt-get install ros-noetic-jderobot-assets
```

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

|         | Noetic | Melodic | Kinetic |
|:-------:|:-------:|:-------:|:-------:|
| Branch  | [`noetic-devel`](https://github.com/JdeRobot/assets/tree/noetic-devel) | [`master`](https://github.com/JdeRobot/assets/tree/master)| [`master`](https://github.com/JdeRobot/assets/tree/master) |
| Status  | supported | supported | EOL |
| Version | [version](http://repositories.ros.org/status_page/ros_noetic_default.html?q=jderobot_assets) | [version](http://repositories.ros.org/status_page/ros_melodic_default.html?q=jderobot_assets)| [version](http://repositories.ros.org/status_page/ros_kinetic_default.html?q=jderobot_assets) |

## ROS Buildfarm

### Ubuntu

|         |  Noetic Focal  |  Melodic Bionic |  Kinetic Xenial  |
|:-------:|:--------------:|:---------------:|:----------------:|
| source | [![Build Status](http://build.ros.org/buildStatus/icon?job=Nsrc_uF__jderobot_assets__ubuntu_focal__source)](http://build.ros.org/job/Nsrc_uF__jderobot_assets__ubuntu_focal__source/) | [![released](http://build.ros.org/buildStatus/icon?job=Msrc_uB__jderobot_assets__ubuntu_bionic__source)](http://build.ros.org/job/Msrc_uB__jderobot_assets__ubuntu_bionic__source/) | [![released](http://build.ros.org/buildStatus/icon?job=Ksrc_uX__jderobot_assets__ubuntu_xenial__source)](http://build.ros.org/job/Ksrc_uX__jderobot_assets__ubuntu_xenial__source/)| 
| bin amd64 | [![Build Status](http://build.ros.org/buildStatus/icon?job=Nbin_uF64__jderobot_assets__ubuntu_focal_amd64__binary)](http://build.ros.org/job/Nbin_uF64__jderobot_assets__ubuntu_focal_amd64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_uB64__jderobot_assets__ubuntu_bionic_amd64__binary)](http://build.ros.org/job/Mbin_uB64__jderobot_assets__ubuntu_bionic_amd64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uX64__jderobot_assets__ubuntu_xenial_amd64__binary)](http://build.ros.org/job/Kbin_uX64__jderobot_assets__ubuntu_xenial_amd64__binary/)| 
| bin i386 | n/a | n/a | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uX32__jderobot_assets__ubuntu_xenial_i386__binary)](http://build.ros.org/job/Kbin_uX32__jderobot_assets__ubuntu_xenial_i386__binary/)| 
| dev amd64 | [![Build Status](http://build.ros.org/buildStatus/icon?job=Ndev__jderobot_assets__ubuntu_focal_amd64)](http://build.ros.org/job/Ndev__jderobot_assets__ubuntu_focal_amd64/) | [![released](http://build.ros.org/buildStatus/icon?job=Mdev__jderobot_assets__ubuntu_bionic_amd64)](http://build.ros.org/job/Mdev__jderobot_assets__ubuntu_bionic_amd64/)| [![released](http://build.ros.org/buildStatus/icon?job=Kdev__jderobot_assets__ubuntu_xenial_amd64)](http://build.ros.org/job/Kdev__jderobot_assets__ubuntu_xenial_amd64/)|
| bin arm64 | [![Build Status](http://build.ros.org/buildStatus/icon?job=Nbin_ufv8_uFv8__jderobot_assets__ubuntu_focal_arm64__binary)](http://build.ros.org/job/Nbin_ufv8_uFv8__jderobot_assets__ubuntu_focal_arm64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_ubv8_uBv8__jderobot_assets__ubuntu_bionic_arm64__binary)](http://build.ros.org/job/Mbin_ubv8_uBv8__jderobot_assets__ubuntu_bionic_arm64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uxv8_uXv8__jderobot_assets__ubuntu_xenial_arm64__binary)](http://build.ros.org/job/Kbin_uxv8_uXv8__jderobot_assets__ubuntu_xenial_arm64__binary/) |
| bin armhf | [![Build Status](http://build.ros.org/buildStatus/icon?job=Nbin_ufhf_uFhf__jderobot_assets__ubuntu_focal_armhf__binary)](http://build.ros.org/job/Nbin_ufhf_uFhf__jderobot_assets__ubuntu_focal_armhf__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_ubhf_uBhf__jderobot_assets__ubuntu_bionic_armhf__binary)](http://build.ros.org/job/Mbin_ubhf_uBhf__jderobot_assets__ubuntu_bionic_armhf__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Kbin_uxhf_uXhf__jderobot_assets__ubuntu_xenial_armhf__binary)](http://build.ros.org/job/Kbin_uxhf_uXhf__jderobot_assets__ubuntu_xenial_armhf__binary/) |


### Debian

|         | Noetic Buster  |  Melodic Stretch   | 
|:-------:|:--------------:|:------------------:|
| source | [![Build Status](http://build.ros.org/buildStatus/icon?job=Nsrc_dB__jderobot_assets__debian_buster__source)](http://build.ros.org/job/Nsrc_dB__jderobot_assets__debian_buster__source/) | [![released](http://build.ros.org/buildStatus/icon?job=Msrc_dS__jderobot_assets__debian_stretch__source)](http://build.ros.org/job/Msrc_dS__jderobot_assets__debian_stretch__source/) | 
| bin amd64 | [![Build Status](http://build.ros.org/buildStatus/icon?job=Nbin_db_dB64__jderobot_assets__debian_buster_amd64__binary)](http://build.ros.org/job/Nbin_db_dB64__jderobot_assets__debian_buster_amd64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_ds_dS64__jderobot_assets__debian_stretch_amd64__binary)](http://build.ros.org/job/Mbin_ds_dS64__jderobot_assets__debian_stretch_amd64__binary/) | 
| bin arm64 | [![Build Status](http://build.ros.org/buildStatus/icon?job=Nbin_dbv8_dBv8__jderobot_assets__debian_buster_arm64__binary)](http://build.ros.org/job/Nbin_dbv8_dBv8__jderobot_assets__debian_buster_arm64__binary/) | [![released](http://build.ros.org/buildStatus/icon?job=Mbin_dsv8_dSv8__jderobot_assets__debian_stretch_arm64__binary)](http://build.ros.org/job/Mbin_dsv8_dSv8__jderobot_assets__debian_stretch_arm64__binary/) |
| dev amd64 | [![Build Status](http://build.ros.org/buildStatus/icon?job=Ndev_db__jderobot_assets__debian_buster_amd64)](http://build.ros.org/job/Ndev_db__jderobot_assets__debian_buster_amd64/) | n/a |


<!-- pr amd64 ubuntu focal -->
<!-- [![Build Status](http://build.ros.org/buildStatus/icon?job=Npr__jderobot_assets__ubuntu_focal_amd64)](http://build.ros.org/job/Npr__jderobot_assets__ubuntu_focal_amd64/) -->

<!-- pr amd64 debian buster -->
<!-- [![Build Status](http://build.ros.org/buildStatus/icon?job=Npr_db__jderobot_assets__debian_buster_amd64)](http://build.ros.org/job/Npr_db__jderobot_assets__debian_buster_amd64/) -->
