#
# Makefile to build a docker image with the specified name.
#
NAME="personalrobotics/ros-openrave:use_ppa"

build: Dockerfile
	docker build -t $(NAME) .

clean:
	docker rmi $(NAME)
