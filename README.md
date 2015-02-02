# COMS 6998-03 HUMANOID ROBOTS, SPRING 2015
# Columbia University


## Getting Started

```bash
$ cd ~
$ git clone git@github.com:HumanoidRobotics/assignment_1.git
$ cd assignment_1
$ source /opt/ros/hydro/setup.bash
$ catkin_make
$ source devel/setup.bash
```

## Runing the Demo code
First, bring up Gazebo, Moveit and the PR2
```bash
$ roslaunch assigment_launch pr2_gazebo_moveit.launch
```

Then run the individual demos with any of the following:
```bash
$ rosrun move_arm move_arm
$ rosrun move_base move_base
$ rosrun move_gripper move_gripper
$ rosrun move_head move_head
```

##Your Solution

In order to test your code, please run:
```bash
$ roslaunch assigment_launch pr2_gazebo_moveit.launch
```

Then:
```bash
$ rosrun pickup_object pickup_object
```

We will grade your assignment by running:
```bash
$ roslaunch assigment_launch assignment_1.launch
```
