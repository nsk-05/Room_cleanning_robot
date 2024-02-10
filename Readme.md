# Repo for simple room cleaning robot

## INSTALLATION 
    mkdir -p ~/Floor_cleaner_ws/src
    cd ~/Floor_cleaner_ws/src
    git clone {this branch}
### Dependency installation
    sudo apt install ros-noetic-grid-map-ros ros-noetic-grid-map-core ros-noetic-grid-map-rviz-plugin ros-noetic-grid-map-visualization ros-noetic-move-base-flex
#### Download full_coverage_path_planner and tracking_pid from git and place it in ~/Floor_cleaner_ws/src  
    https://github.com/nobleo/full_coverage_path_planner
    https://github.com/nobleo/tracking_pid.git

### Build
    cd ~/Floor_cleaner_ws
    catkin_make

### Starting robot
    roslaunch robot_gazebo gazebo.launch

### Cleaning complete map
    roslaunch robot_navigation cleaning.launch


