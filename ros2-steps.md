# ROS2

## In tortoisebot: open several connections

    ssh tortoisebot@192.168.18.122

source!!!

    source /opt/ros/galactic/setup.bash
    source ~/ros2_ws/install/setup.bash

**terminal 1**

    ros2 launch tortoisebot_bringup autobringup.launch.py use_sim_time:=False exploration:=True

**terminal 2**

    ros2 run tortoisebot_control teleop_twist_keyboard

### Others

Save the map

    ros2 run nav2_map_server map_saver_cli -f NAME_OF_MAP_FILE.yaml

For autonomous navigation

    ros2 launch tortoisebot_bringup autobringup.launch.py use_sim_time:=False exploration:=False map:=/home/../NAME_OF_MAP_FILE.yaml

## In The Construct's computer:

    cd ~/ros2_ws/src/
    git clone -b ros2-galactic https://github.com/rigbetellabs/tortoisebot.git

source!!!

    source /opt/ros/galactic/setup.bash
    source ~/ros2_ws/install/setup.bash

**terminal 1**

ros2 launch tortoisebot_description rviz.launch.py



