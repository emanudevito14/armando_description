Create folder named armando_description and putting all files and folders into it.
Place armando_description in ros2_ws/src.

In ros2_ws, open a terminal and build the package:
```bash
export IGN_GAZEBO_RESOURCE_PATH=$IGN_GAZEBO_RESOURCE_PATH:~/ros2_ws/src/armando_description/meshes
export IGN_SYSTEM_PLUGIN_PATH=$IGN_SYSTEM_PLUGIN_PATH:~/ros2_ws/install/armando_description/lib
colcon build --packages-select armando_description
```
Open a new terminal in ros2_ws and source the setup script:
```bash
source install/setup.bash
```
Open another terminal in ros2_ws and launch the armando_hardware.launch.py file:
```bash
ros2 launch armando_description armando_gazebo.launch.py
```
Open new terminal
```bash
ros2 run rqt_image_view rqt_image_view
```
next to refresh symbol select /videocamera
