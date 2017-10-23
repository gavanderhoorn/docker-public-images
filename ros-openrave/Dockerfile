FROM ros:indigo-ros-base
MAINTAINER Pras Velagapudi <pkv@cs.cmu.edu>
ENV DEBIAN_FRONTEND noninteractive

# Add the personalrobotics PPA
# TODO: do this without software-properties-common
RUN apt-get update \
    && apt-get install -y --no-install-recommends software-properties-common \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Install OpenRAVE and clear cache.
RUN add-apt-repository -y ppa:personalrobotics/ppa \
    && apt-get update \
    && apt-get install -y --no-install-recommends pr-openrave \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
