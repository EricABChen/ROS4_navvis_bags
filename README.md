# Lab3: ecse473_f23_axc1293_navvis_bags

## Package description
This repo is a ROS package that contains the bags and playbacks of a navvis robot routing within Glennan Bldg

## Dependency:
In order to run/view this model, the listed dependencies MUST be satisfied:
-  ROS(Noetic)
-  gazebo-plugins
-  ROS velodyne-description
-  ROS map server (place under `catkin_ws/src`)
-  map file (view map file section for detailed detailed information)

## Map File
The data of this implementation comes from a private dataset and is NOT included in this implementation, by default, the data should be stored within `~/catkin_ws/src/<packagename>/raw_bags/`

## RUN
To view the robot model in RVIZ, you need to first download this package into

`~/catkin_ws/src/`

Build the package with

`catkin_make`

Then source:

`source catkin_ws/devel/setup.bash`

MAKE SURE the data is inside folder `raw_bags`,then launch the model with RVIZ:

`roslaunch navvis_bags navvis_bags.launch`

## Param

`"bag_path": The path of your own bag data`

Note: if the data is stored within `~/<packagename>/raw_bags/`, you can launch the model without configuring this param

## To view the navvis_robot model:

`roslaunch navvis_description navvis_launch.launch use_xacro:=true`

