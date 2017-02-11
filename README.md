# depth_nav_tools
Set of tools for mobile robot navigation with depth sensor, for example 
Microsoft Kinect.

Package depth_nav_tools contains following packages:
- laserscan_kinect -- converts depth image to laser scan (LaserScan). 
It finds smallest value of distance in each column of depth image 
and converts it to polar coordinates. Moreover, package provides features 
like ground removing from scan and sensor tilt compensation in distance values, 
but it is necessary to know height of sensor optical center and tilt angle in frame of ground.

- depth_sensor_pose -- detects ground plane on depth image and estimate 
                       height and tilt angle of depth sensor.

- cliff_detector -- detects negative objects like a cliff or downstairs.

- nav_layer_from_points -- creates navigation costmap layer based on received
                           points.
- depth_nav_msgs -- specific messages for other packages.

## Deprecated
Please use version of package for ROS Kinetic.

## ROS Documentation 
A more detailed, standard ROS-style documentation of this package can be found on the ROS wiki at:
http://wiki.ros.org/depth_nav_tools
