# BarelangFC AdultSize Gazebo Simulation Model

**Setup Workspace**

Install dependencies

```bash
sudo apt install ros-noetic-ros-control
sudo apt install ros-noetic-ros-controllers
```

Clone simulation package

```bash
cd ~
mkdir -p barelangfc/src
cd barelangfc/src
git clone -b noetic-devel https://github.com/ROBOTIS-GIT/DynamixelSDK.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Framework.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Framework-msgs.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Math.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Utility.git
git clone https://github.com/roboticsgroup/roboticsgroup_gazebo_plugins.git
git clone https://github.com/BarelangFC/BarelangFC-AdultSize-Simulation.git
cd ..
catkin_make
source devel/setup.bash 
```

**Running Simulation**

```bash
roslaunch humanoid_manager humanoid_gazebo.launch
roslaunch humanoid_gazebo humanoid_gazebo.launch
```

**Moving Joint**
Example command for moving head pan joint
```bash
rostopic pub /robotis/set_joint_states sensor_msgs/JointState "header:
  seq: 0
  stamp: {secs: 0, nsecs: 0}
  frame_id: ''
name: ['head_pan']
position: [1]
velocity: [0]
effort: [0]" 
```

**Link Part Files**

Link design location : Adult Size\Assy fix\Assy_Leg.SLDASM \
https://drive.google.com/file/d/1JB6ATBQTLTad41ta_7nGuA0eSaegAw7J/view?usp=sharing
