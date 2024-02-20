# Installation steps
- Ubuntu 22.04
- Ros2 installed locally (I built iron from [source](https://docs.ros.org/en/iron/Installation/Alternatives/Ubuntu-Development-Setup.html))
- teleop-twist-keyboard installed: `sudo apt-get install ros-iron-teleop-twist-keyboard`
- rviz2 installed: `sudo apt install ros-iron-rviz2`
- xacro and joint GUI publisher (for testing) installed: `sudo apt install ros-iron-xacro ros-iron-joint-state-publisher-gui`
- Gazebo/Ros integration installed: `sudo apt-get install ros-iron-ros-gz`

# Running
From the root directory (daniel@daniel-MacBookPro:~/ros2-two-wheeled-bot$):
```
colcon build
source install/setup.bash
ros2 launch two_wheeled_robot launch_sim.launch.py
```

From another terminal:
```
source ~/ros2_iron/install/setup.bash
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```
