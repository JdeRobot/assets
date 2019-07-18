cmake_minimum_required(VERSION 2.8.3)
project(jderobot_assets)

find_package(catkin REQUIRED COMPONENTS)
catkin_package()

install(DIRECTORY models worlds
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)