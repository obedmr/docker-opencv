docker-opencv
=============
This provides a container for doing OpenCV development

Build
-----
```
    docker build -t obedmr/opencv .
```

Or just pull it from Dockerhub
------------------------------
```
    docker pull obedmr/opencv
```

Run the OpenCV Container
------------------------
```
  # Allow docker container display X applications
  xhost local:root
  # Start OpenCV container in --privileged mode
  docker run --rm -it --privileged \
         -v /tmp/.X11-unix/:/tmp/.X11-unix \
	 -e DISPLAY=$DISPLAY obedmr/opencv bash

```

