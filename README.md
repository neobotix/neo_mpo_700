# ROS configuration and launch files for Neobotix MPO-700

This package contains configuration and launch files for Neobotix MPO-700.

![Neobotix MPO-700](http://www.neobotix-roboter.de/fileadmin/_processed_/2/5/csm_omnidirektional-MPO-700-Hauptansicht_02_45470f9829.jpg)![Neobotix MMO-700](http://www.neobotix-roboter.de/fileadmin/_processed_/9/8/csm_MMO-700-UR10-Main_01_fdf4bc6d22.jpg)

The omnidirectional [MPO-700](http://www.neobotix-robots.com/omnidirectional-robot-mpo-700.html) is the ideal base for high-end service robots. Its four Omni-Drive-Modules enable it to move extremely smoothly into any direction. This robot is even capable of rotating freely while driving to its destination. The Omni-Drive-Modules of the MPO-700 feature important benefits compared to other omnidirectional drive kinematics, like for example the MPO-500's Mecanum wheels.

* Fully omnidirectional manoeuvrability
* Very steady movements
* High stability and payload
* Compact, easily integrated drive units

This makes the MPO-700 a premium alternative for applications that require omnidirectional movements without the limitations of traditional kinematics.

# Contact information

For more information please visit our website at www.neobotix-robots.com. 
If you have any questions, just get in touch with us:
* General information: http://www.neobotix-robots.com/company-contact.html
* ROS related questions: ros@neobotix.de


# Installation

1. Create a catkin workspace ([tutorial](http://wiki.ros.org/catkin/Tutorials/create_a_workspace))

2. Download all packages listed under "Additionally required Neobotix-ROS-Packages" into your workspace

3. IMPORTANT! Delete all not used packages downloaded in step 2!

4. Install all packages listed under "Additionally required third party ROS-Packages"

5. Build your workspace


## Additionally required Neobotix-ROS-Packages:

Hardware connection: ![neo_relayboard_v2](https://github.com/neobotix/neo_relayboard_v2)

Kinematic:  ![cob_driver](https://github.com/neobotix/cob_driver) and ![cob_common](https://github.com/neobotix/cob_common)

Laserscanner: ![cob_sick_s300](https://github.com/neobotix/neo_driver)

Scan-Merge: ![cob_scan_unifier](https://github.com/neobotix/neo_driver)

Teleoperation: ![neo_teleop](https://github.com/neobotix/neo_control)

Homing and Recover: ![neo_auto_recover](https://github.com/neobotix/neo_control)

Msgs: ![neo_msgs](https://github.com/neobotix/neo_msgs)

Srvs: ![neo_srvs](https://github.com/neobotix/neo_srvs)

## Additionally required third party ROS-Packages:

Joystick: [joy](http://wiki.ros.org/joy)

MoveBase: [move_base](http://wiki.ros.org/move_base) and [move_base_msgs](http://wiki.ros.org/move_base)

SLAM: [gmapping](http://wiki.ros.org/gmapping)

AMCL: [amcl](http://wiki.ros.org/amcl)

## Usage:

1. Edit the configuration of each ROS-Node to meet your needs 

2. Use the bringup.launch file for basic startup

3. Use the navigation.launch file for starting up MoveBase and SLAM or AMCL

4. Create your own .launch file

### ROSlaunch files:

Bringup: ![bringup.launch](https://github.com/neobotix/neo_mpo_700/blob/indigo/launch/mpo/bringup.launch)

Navigation with SLAM: ![navigation_basic_slam.launch](https://github.com/neobotix/neo_mpo_700/blob/master/launch/mpo_700/navigation_basic_slam.launch)

Navigation with AMCL: ![navigation_basic_amcl.launch](https://github.com/neobotix/neo_mpo_700/blob/master/launch/mpo_700/navigation_basic_amcl.launch)

### Configuration:

For each used ROS-Node there is a Folder in configs
