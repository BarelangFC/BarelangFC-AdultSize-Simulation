# Barelang FC Sim

**Setup Workspace**

```bash
cd ~
mkdir -p barelangfc/src
cd barelangfc/src
git clone -b noetic-devel https://github.com/ROBOTIS-GIT/DynamixelSDK.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Framework.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Framework-msgs.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Math.git
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Utility.git
cd ..
catkin_make
source devel/setup.bash 
```

**Running Simulation**

```bash
roslaunch humanoid_gazebo humanoid_gazebo.launch
roslaunch humanoid_manager humanoid_gazebo.launch
```

**Link Part Files**

Link design location : Adult Size\Assy fix\Assy_Leg.SLDASM \
https://drive.google.com/file/d/1JB6ATBQTLTad41ta_7nGuA0eSaegAw7J/view?usp=sharing
