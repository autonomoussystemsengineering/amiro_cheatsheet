# AMiRo Cheatsheet

## Install RSB<->ROS setup
```
# Install RSB/RST/RSC in version 0.17 from http://docs.cor-lab.de/
# Install ROS Kinetic
cd ~
mkdir -p catkin_ws/src
cd catkin_ws/src
source /opt/ros/kinetic/setup.bash
git clone https://github.com/autonomoussystemsengineering/amiro_bridges.git
git clone https://github.com/autonomoussystemsengineering/amiro_msgs.git

# Create a rsb.conf in ~/.config/rsb.conf e.g.

```
[plugins.cpp]
load = rsbspread

[transport.spread]
host    = alice.techfak.uni-bielefeld.de
# host    = localhost
port    = 4803
enabled = 1

[transport.inprocess]
enabled = 0

[transport.socket]
enabled = 0
```


# Install amiro_senseact

# Install or source cross compiler
git clone https://github.com/autonomoussystemsengineering/amiro_senseact.git
cd amiro_senseact
source source.sh
cd project/demo/sense_act_demo
./install.sh

# copy binariers to AMiRo and run start.sh
```
