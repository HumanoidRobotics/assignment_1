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
$ roslaunch assignment_launch pr2_gazebo_moveit.launch
```

Then run the individual demos with any of the following:
```bash
$ rosrun move_arm move_arm
$ rosrun move_base move_base
$ rosrun move_gripper move_gripper
$ rosrun move_head move_head
```

##Your Solution

Your solution will go in either pickup_object.cpp or pickup_object.py in the pickup_object package.  We have provided the
move_* packages to provide code to get you started.  Please make sure that the correct line is uncommented in the pickup_object.launch
file depending on whether you use python or C++.

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
$ roslaunch assignment_launch assignment_1.launch
```

For this assigment we expect you to have the PR2 navigate to the table, and pick the cup off the table.  It is ok if the cup
falls out of the PR2's gripper after several seconds. 

##Submission
In order to submit your your code, please run the following:
```bash
$ cd ~/assignment_1
$ tar czf [YOUR UNI]_assignment_1.tar.gz src
```

Then submit the compressed src directory to courseworks.