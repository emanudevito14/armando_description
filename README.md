Create a folder named armando_description and put these files and folders into it.
Place armando_description in ros2_ws/src.

In ros2_ws, open a terminal and build the package:
```bash
colcon build --packages-select armando_description
```
Open a new terminal in ros2_ws and source the setup script:
```bash
source install/setup.bash
```
Open another terminal in ros2_ws and launch the armando_display.launch.py file:
```bash
ros2 launch armando_description armando_display.launch.py
```
