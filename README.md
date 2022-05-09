# XBOX360
**安裝Kinect驅動程式**
* 安裝openni
> $sudo apt-get install ros-melodic-openni-camera ros-melodic-openni-launch
* 安裝freenect
> $sudo apt-get install ros-melodic-freenect-camera ros-melodic-freenect-stack ros-melodic-freenect-launch

**安裝rviz**
> $sudo apt-get install ros-melodic-rviz

**安裝RTAB-Map**
> $sudo apt-get install ros-melodic-rtabmap-ros

**啟動XBOX360從rtab-map & rviz檢視**
> $roscore
> 
> $roslaunch freenect_launch freenect.launch depth_registration:=true data_skip:=2
> 
> $roslaunch rtabmap_ros rtabmap.launch rtabmap_args:="--delete_db_on_start"
> 
> $rviz
