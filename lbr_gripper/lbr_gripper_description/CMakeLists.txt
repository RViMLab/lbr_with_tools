cmake_minimum_required(VERSION 3.10.2)
project(lbr_gripper_description)

find_package(catkin REQUIRED)
catkin_package()

install(DIRECTORY urdf DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
