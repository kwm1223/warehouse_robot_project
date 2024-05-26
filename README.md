# warehouse_robot_project
The repo for multi-robot project in warehouse, a project of 'The Self-driving Dev Course'

## member

- zozibush([Github](https://github.com/zozibush)) : AGV
- woong137([Github](https://github.com/woong137)) : AMR
- kwm1223([Github](https://github.com/kwm1223)) : master

## Go1
- terminal 1
`roslaunch unitree_gazebo robot_simulation.launch`

- terminal 2
`rosrun unitree_guide junior_ctrl`

press the keys '2' and '4' to set the robot in trotting mode
'W', 'A', 'S', 'D' keys to control the translation of the robot, and press the 'J', 'L' keys to control the rotation of the robot

- terminal 3
`roslaunch unitree_navigation slam.launch rname:=go1 rviz:=true algorithm:=gmapping`

- terminal 4
`rosrun map_server map_saver -f ~/warehouse_robot_project/src/ros_unitree/unitree_guide/unitree_navigation/maps/aws`
