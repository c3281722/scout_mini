cmake_minimum_required(VERSION 2.8.3)
project(scout_description)

find_package(catkin REQUIRED COMPONENTS roslaunch)

catkin_package()

if(CATKIN_ENABLE_TESTING)
  roslaunch_add_file_check(...)
endif()

install(
  DIRECTORY launch meshes urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
