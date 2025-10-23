Create folder armando_description and put these file and folder into it. Put armando_description in ros2_ws/src. 
In ros2_ws open terminal and build the ros2_ws's package:
```bash
colcon build --packages-select armando_description ```
Open new terminal and execute this in ros2_ws:
```bash
source install/setup.bash ```
Open another terminal and launch armando_display.launch.py:
```bash
ros2 launch armando_description armando_display.launch.py ```
