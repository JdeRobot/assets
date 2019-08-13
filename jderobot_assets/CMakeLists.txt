cmake_minimum_required(VERSION 2.8.3)
project(jderobot_assets)

find_package(catkin REQUIRED COMPONENTS
  turtlebot3_description
  turtlebot3_gazebo
)

find_package(gazebo REQUIRED)

catkin_package()

install(DIRECTORY models worlds perspectives urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)