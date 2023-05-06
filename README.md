# ROS TURTLEBOT 3 Docker Container

Sets up a base docker image for the rosturtlebot 3   in Gazebo that you can control via teleop_twist and view in rviz.

This image does require x11 support and a GPU is recommended. The easiest way to run this image is through [rocker][rocker].

## Install

### Prerequisites

- [Docker][docker]
- [Nvidia Container Toolkit][nvidia-docker]
- [Rocker][rocker]

After installing installing the docker and nvidia prerequisites, install [rocker][rocker]:

```bash
sudo apt install python3-rocker
```

### Running the image

```
rocker --nvidia --x11  --volume /dev/dri -- docker_turtlebot3_simulations:latest
```

[docker]: https://docs.docker.com/engine/install/ubuntu/
[nvidia-docker]: https://github.com/NVIDIA/nvidia-docker
[rocker]: https://github.com/osrf/rocker
