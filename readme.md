# Moveit config package for UR5e + Schunk EGP50 Gripper

## Simulation

1. Start the sim:  
`roslaunch ur_manipulation gazebo_ur5e_egp50.launch`

2. Start the moveit config + rviz:  
`roslaunch ur5e_egp50_moveit_config ur5e_egp50_moveit_planning_execution.launch sim:=true`

## Real robot 

1. Start the robot driver with this :   
`roslaunch ur_manipulation ur5e_bringup.launch`   
Once done, in the Teach Pendant, go to Program > URCaps and tap on External Control to add it to the program.    
Start this program by pressing the play button at the bottom, verify in the driver launch window if this was recognised.     
Robot IP is hard coded in launch, change as needed.

2. Start Moveit + RVIZ :   
`roslaunch ur5e_egp50_moveit_config ur5e_egp50_moveit_planning_execution.launch`   

3. Start the application node :    
`roslaunch ur_manipulation seher_demo.launch`  
