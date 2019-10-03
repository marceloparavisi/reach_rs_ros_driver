cmake_minimum_required(VERSION 2.8.3)
project(reach_rs_driver)

find_package(catkin REQUIRED)

catkin_python_setup()
catkin_package()

install(PROGRAMS
  scripts/reach_rs_driver_node.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)


install(DIRECTORY launch/
   DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch)
