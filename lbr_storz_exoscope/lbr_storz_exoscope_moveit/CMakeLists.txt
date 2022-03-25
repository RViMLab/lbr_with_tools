cmake_minimum_required(VERSION 3.5)
project(lbr_storz_exoscope_moveit)

find_package(ament_cmake REQUIRED)

install(
    DIRECTORY launch config
    PATTERN "setup_assistant.launch" EXCLUDE
    DESTINATION share/${PROJECT_NAME}
)

ament_package()
