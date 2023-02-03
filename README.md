# Ned2_Control
Control Niryo Ned2

## Documentations
Official documentations: https://docs.niryo.com/dev/ros/v4.1.0/en/index.html

Git Repo (this one basically covers everything :) created by Matthew Stachyra: https://github.com/tufts-ai-robotics-group/ned2

## Connect to Ned2
1. SSH into Ned2's Raspberry Pi 4
    
    Check list:
    - Any computer with a terminal
    - Ned2 (Physical arm :)

    Steps:
    - Press the button behind to turn on Ned2 (make sure the security button (big red button) is released)
    - Connect to the hotspot on Ned via WiFi. It will show up as something like "NiryoRobot" followed by some characters. The password is "niryorobot".
    - Type in command: $ ssh niryo@10.10.10.10
    - Password "robotics"
    - Updon successful connection, you can see the robot printed out followed by "Welcome to Ned 2 by Niryo".

    
    - Turn off Ned2: 
        - Use freemotion button to put the arm to a rested position on the table or else it will fall and hit the table when power off
        - Type in command to stop the robot’s program: $ sudo service niryo_robot_ros stop
        - Type in command to exit the ssh connection: $ exit
        - Turning off Ned2 by holding the power button

2. Use simulation on your own computer
    
    Check List:
    - Ubuntu 18.04
    - ROS melodic
    - Niryo ROS Stack 
    (install the Niryo Robot Stack on an Ubuntu 18 OS following https://docs.niryo.com/dev/ros/v4.1.0/en/source/installation/ubuntu_18.html)

    Steps:
    - 


## Control Ned2 using Python ROS Wrapper
- niryo_robot_python_ros_wrapper: https://docs.niryo.com/dev/ros/v4.1.0/en/source/ros_wrapper.html
- pyniryo: https://docs.niryo.com/dev/pyniryo/v1.1.0/en/source/examples/examples_basics.html
