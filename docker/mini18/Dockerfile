FROM ubuntu:18.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get --yes update
RUN apt-get --yes install \
    apt-utils git sudo g++ make gnupg gdb cmake \
    x11-apps mesa-utils \
    nano emacs terminator lsb-release gnuplot

# this is only to speed up
# the make installUbuntuAll would do the same in the test shell...

RUN apt-get --yes install \
     liblapack-dev libf2c2-dev libeigen3-dev \
     libx11-dev libglfw3-dev libglew-dev freeglut3-dev graphviz-dev \
     libjsoncpp-dev libassimp-dev libqhull-dev libann-dev 

WORKDIR /root
