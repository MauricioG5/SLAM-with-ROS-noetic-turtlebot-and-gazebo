# SLAM-with-turtlebot-and-gazebo

To use gazebo and turtlebot to visualize SLAM on ROS, follow the following steps:

1. Download hokuyo node from: https://github.com/ros-drivers/hokuyo_node
2. Download turtlebot using sudo apt-get install <turtlebot or turtlebot3>
3. Download gazebo plugins from: http://wiki.ros.org/gazebo_plugins
4. Follow this tutorial: https://joshi-bharat.github.io/posts/adding-hokuyo-lasers
5. Type on the terminal: export TURTLEBOT3_MODEL=burger each time before running the simulation
6. Type roslaunch turtlebot3_gazebo turtlebot3<world_name>.launch to run the simulation. e.g. (roslaunch turtlebot3_gazebo turtlebot3_empty_world.launch)
