# ardrone_autonomy for multiple drones

## Under Development

Run as 

...
rosrun ardrone_autonomy ardrone_driver --ip 192.168.0.134 --prefix "ardrone_2" 
rosrun ardrone_autonomy ardrone_driver --ip 192.168.0.134 --prefix "ardrone_2" -
-nodrone
...

## Install

You can download using github 

...
mkdir driver
cd driver
git clone https://github.com/noyogi/Autonomy-Multidrone.git
cd ..
rosdep install --from-paths src -i
catkin_make
cp src/moveToLib devel/src/ardronelib/ARDroneLib/Soft/Lib/ardrone_tool/*
...


You need to manually update the library to support the driver


[ROS](http://ros.org) Driver for [Parrot AR-Drone](http://ardrone2.parrot.com/) 1.0 & 2.0 Quadrocopters

* Documentation: http://ardrone-autonomy.readthedocs.org/
* ROS wiki page: http://wiki.ros.org/ardrone_autonomy
* Code API: http://docs.ros.org/indigo/api/ardrone_autonomy/html
* Patched _ARDroneLib_ repository: https://github.com/AutonomyLab/ardronelib
* Author: [Mani Monajjemi](http://mani.im) ([Autonomy Lab](http://autonomylab.org), [Simon Fraser University](http://www.sfu.ca)) + [other contributers](http://ardrone-autonomy.readthedocs.org/en/latest/contributers.html)

## Build Status

* ROS Build farm (_Jade_): [![Build Status](http://build.ros.org/buildStatus/icon?job=Jdev__ardrone_autonomy__ubuntu_trusty_amd64)](http://build.ros.org/job/Jdev__ardrone_autonomy__ubuntu_trusty_amd64/)
* ROS Build farm (_Indigo_): [![Build Status](http://build.ros.org/buildStatus/icon?job=Idev__ardrone_autonomy__ubuntu_trusty_amd64)](http://build.ros.org/job/Idev__ardrone_autonomy__ubuntu_trusty_amd64/)
* Travis (_Jade_/_Indigo_): [![Build Status](https://travis-ci.org/AutonomyLab/ardrone_autonomy.svg?branch=indigo-devel)](https://travis-ci.org/AutonomyLab/ardrone_autonomy)

