# LBR With Tools
KUKA LBR med7 R800 robot with tools.

## Build
```shell
mkdir -p lbr_with_tools_ws/src && cd lbr_with_tools_ws && \
wget https://raw.githubusercontent.com/RViMLab/lbr_with_tools/foxy/lbr_with_tools/repos.yml -P src && \
vcs import src < src/repos.yml && \
colcon build
```

## Launch
```shell
package=lbr_da_vinci_endoscope  # where package is any of the package here
source install/setup.bash && \
ros2 launch lbr_description view_robot.launch.py description_package:=${package}_description description_file:=urdf/${package}.urdf.xacro
```
