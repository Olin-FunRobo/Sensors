## LIDAR

### (Depricated) Installing and Testing

```bash
# Install ROS Hokuyo Driver
sudo apt-get install ros-indigo-hokuyo-node

# If roscore isn't running, instantiate it:
roscore &

# Run the node; replace /dev/ttyACM0 with your device serial port.
rosrun hokuyo_node hokuyo_node /dev/ttyACM0
```

### Installing and Testing

Follow the same sequence as above, but install a different ROS driver:

```bash
sudo apt-get install ros-indigo-urg-node
rosrun 
```

and run the node as follows:

```bash
rosrun urg_node urg_node _serial_port:=/dev/ttyACM0
```

### Visualization

```bash
# In this directory
rviz -d lidar.rviz 
```

### Sample Data

If you want to get a feel of what kind of data you'd be collecting:

```bash
rosbag play lidar.bag
```
And run the visualization node.
