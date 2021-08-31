# udacity-where-am-i
## Project 3: Where am I? From Udacity Robotics Engeneer Nanodegree

### How to install
Simply put all three packages to the catkin_ws/src directory and run
```
catkin_make
```
from catkin_ws directory. This should build all the packages and Ackermann steering plugin without problems!

### How to use
First you need to launch the world simulation with
```
roslaunch my_robot world.launch
```
Then you need to launch AMCL localization node with
```
roslaunch my_robot amcl.launch
```
And you're good to go!

You can control the robot by creating 2DNavigation goal in Rviz.

You can also run keyboard teleop node to control the robot manualy with
```
rosrun teleop_twist_keyboard teleop_twist_keyboard
```


The robot starts in the hallway, so it is hard to locolize it right away. But as soon as the robot enters one of the rooms localization solution should converge quickly!


### Known Issues
#### Gazebo crash
Sometimes gazebo just crashes - simply relaunch it.
