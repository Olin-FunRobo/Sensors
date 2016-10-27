## Install Camera Drivers

```bash
sudo apt-get install ros-indigo-libuvc\*
sudo apt-get install ros-indigo-uvc-camera
```

## Image Visualization and Processing Packages

```bash
sudo apt-get install ros-indigo-image-view ros-indigo-image-proc ros-indigo-camera-calibration
```

## Running the Camera

```bash
rosrun uvc_camera uvc_camera_node _device:="/dev/video0" 
```

## Calibrating the Camera

Follow the instructions on [This Tutorial](https://olinrobotics.github.io/Odroid_Setup/arpose#calibrating-the-camera)

## Visualizing the Results

Follow the instructions [here](https://olinrobotics.github.io/Odroid_Setup/arpose#if-arpose-still-fails)
