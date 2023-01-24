# SLAM-with-turtlebot-and-gazebo

To use gazebo and turtlebot to visualize SLAM on ROS, follow the following steps:

1. Download hokuyo node from: https://github.com/ros-drivers/hokuyo_node
2. Download turtlebot using sudo apt-get install turtlebot3
3. Download gazebo plugins from: http://wiki.ros.org/gazebo_plugins
4. Follow this tutorial: https://joshi-bharat.github.io/posts/adding-hokuyo-lasers
5. Type on the terminal: <export TURTLEBOT3_MODEL=burger> each time before running the simulation
6. Type on the terminal <roslaunch turtlebot3_gazebo turtlebot3<world_name>.launch> to run the simulation. e.g. 
> (roslaunch turtlebot3_gazebo turtlebot3_world.launch)


9. To move the robot with WASD, first use the export: export TURTLEBOT3_MODEL=${TB3_MODEL}, then you can run: <roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch>
10. To run the SLAM application, first export: export TURTLEBOT3_MODEL=burger, the you can run: roslaunch turtlebot3_slam turtlebot3_slam.launch
11. https://emanual.robotis.com/docs/en/platform/turtlebot3/simulation/
12. After creating the map using SLAM, you can save it with>

> rosrun map_server map_saver -f ~/maps/world/map

The final arguement defines where the map will be saved

13. Run navigation using:
> roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/maps/world/map.yaml

The final arguement defines where to take the map from 
