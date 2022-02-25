# Moveit config package for UR5e + Schunk EGP50 Gripper

## Simulation

1. Start the sim:  
`roslaunch ur_manipulation gazebo_ur5e_egp50.launch`

2. Start the moveit config + rviz:  
`roslaunch ur5e_egp50_moveit_config ur5e_egp50_moveit_planning_execution.launch sim:=true`
