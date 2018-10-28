# RoboND-Where-am-i
Where-am-i Project

### Step 1/ Source the setup.bash file
'''console
$ source devel/setup.bash
'''

### Step 2/ Launch the Gazebo and RViz environment
$ roslaunch udacity_bot udacity_world.launch
$ roslaunch udacity_bot amcl.launch

### Step 3/ Change parameters in amcl.launch, some parameter files
Change directory in terminal to launch folder and edit amcl.launch file
$ cd ../RoboND-Where-am-i/src/udacity_bot/launch
$ gedit amcl.launch

Change directory in terminal to config folder and edit following files
$ cd ../RoboND-Where-am-i/src/udacity_bot/config
$ gedit costmap_common_params.yaml
$ gedit base_local_planner_params.yaml
$ gedit global_costmap_params.yaml
$ gedit local_costmap_params.yaml

### After changing parameters in amcl.launch, relaunch amcl.launch
$ roslaunch udacity_bot amcl.launch
$ rosrun udacity_bot navigation_goal
