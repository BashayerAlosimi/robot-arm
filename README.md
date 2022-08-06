after installing ROS, using below command to git package for robot arm

1- creating catkin workspace (sudo apt-get install ros-noetic-catkin)

(mkdir -p ~/catkin_ws/src)

(cd ~/catkin_ws/)

(catkin_make)

(cd ~/catkin_ws/src)

2- package for robot arm (git clone https://github.com/smart-methods/arduino_robot_arm.git)

(cd ~/catkin_ws)

7- other important ROS package (rosdep install --from-paths src --ignore-src -r -y)

(sudo apt-get install ros-noetic-moveit)

(sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui)

(sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher)

(sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control)

8- put the source of setup.bash in bashrc file (sudo nano ~/.bashrc)

at the end of the (bashrc) file add the follwing line (source /home/wesam/catkin_ws/devel/setup.bash) then ctrl + o

(source ~/.bashrc)

9- run RViz (roslaunch robot_arm_pkg check_motors.launch)

![](robot%20arm.png)
