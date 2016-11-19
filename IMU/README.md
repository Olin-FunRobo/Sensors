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
rosrun phidgets_imu phidgets_imu_node

# You may have to plug it in while it's waiting
# When you're running for the first time

```

## Running the bag

```bash
rosbag play imu.bag
rviz -d imu.rviz
```

### If RVIZ doesn't work

One of the problems that we've encountered was RViz being unable to load the plugin.

Install the IMU plugin as follows:

```bash
sudo apt-get install ros-indigo-rviz-imu-plugin
```
