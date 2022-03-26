cmake_minimum_required(VERSION 3.5)
project(lbr_storz_exoscope_description)

find_package(ament_cmake REQUIRED)

install(
    DIRECTORY urdf
    DESTINATION share/${PROJECT_NAME}
)

ament_package()
