# SLAM-with-turtlebot-and-gazebo

To use gazebo and turtlebot to visualize SLAM on ROS, follow the following steps:

1. Download hokuyo node from: https://github.com/ros-drivers/hokuyo_node
2. Download turtlebot using sudo apt-get install turtlebot3
3. Download gazebo plugins from: http://wiki.ros.org/gazebo_plugins
4. Follow this tutorial: https://joshi-bharat.github.io/posts/adding-hokuyo-lasers
5. Type on the terminal: export TURTLEBOT3_MODEL=burger each time before running the simulation
6. Type roslaunch turtlebot3_gazebo turtlebot3<world_name>.launch to run the simulation. e.g. (roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch)
7. To move the robot with WASD, first use the export: export TURTLEBOT3_MODEL=${TB3_MODEL}, then you can run: roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
8. To run the SLAM application, first export: export TURTLEBOT3_MODEL=burger, the you can run: roslaunch turtlebot3_slam turtlebot3_slam.launch
9. https://emanual.robotis.com/docs/en/platform/turtlebot3/simulation/
