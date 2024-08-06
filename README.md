

# Set-up

```
cd ~/catkin_ws && colcon build --symlink-install
export TURTLEBOT3_MODEL=waffle
source ~/catkin_ws/install/local_setup.bash
. /usr/share/gazebo/setup.bash
export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:/home/gh/catkin_ws/src/turtlebot3_gazebo_nav2/turtlebot3_simulations/turtlebot3_gazebo/models
```

# Launch
```
ros2 launch nav2_bringup tb3_simulation_launch.py headless:=False
```
