# launch_slam  
Project by [Paul Asquin](https://www.linkedin.com/in/paulasquin/) for Awabot - Summer 2018 paul.asquin@gmail.com  

Launch files used for SLAM technologies benchmarking  

# Installation
```
git clone https://bitbucket.org/awabot/launch_slam/src/master/
```

# Usage  

With this project, you can choose to test only one technology at a time. To do so, you have to run 
```
roscore
```
then play your rosbag with
```
rosbag play PATH_TO_ROSBAG.bag
```
and finally run
```
roslaunch slamTechno/emox_slamTechno.launch
```  
Be sure that your topics matches with those in the launch files. If not, you can remap the launch files.  
  
  
If you want to use the benchmarking mode, install the buggy project (also developped by Paul Asquin), 
open [rosbag_and_buggy.launch](rosbag_and_buggy.launch), indicate PATH_TO_ROSBAG and finally run 
```
roslaunch benchmarking_buggy.launch
```
