# Using the IMU

## Installation

[Link](http://wiki.ros.org/phidgets_drivers)

```bash
cd ~/catkin_ws/src
git clone https://github.com/ccny-ros-pkg/phidgets_drivers.git

sudo apt-get install ros-indigo-libphidgets
# alternatively,
# rosdep install libphidgets
# rosmake libphidgets

rosdep install phidgets_drivers
rosmake phidgets_drivers

roscd
cd ../
catkin_make
sh src/phidgets_drivers/phidgets_api/share/setup-udev.sh
```

## Running

```
rosrun phidgets_imu imu_node

# You may have to plug it in while it's waiting
# When you're running for the first time

```

## Running the bag

```bash
rosbag play imu.bag
rviz -d imu.rviz
```
