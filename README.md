Place armando_gazebo in ros2_ws/src.

In ros2_ws, open a terminal and build the package:
```bash
export IGN_GAZEBO_RESOURCE_PATH=$IGN_GAZEBO_RESOURCE_PATH:~/ros2_ws/src/armando_gazebo/meshes
colcon build --packages-select armando_gazebo
```
Open a new terminal in ros2_ws and source the setup script:
```bash
source install/setup.bash
```
Open another terminal and launch the armando_world.launch.py file:
```bash
ros2 launch armando_gazebo armando_world.launch.py
