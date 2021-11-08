# Barelang FC Sim 
mkdir barelangfc\
cd barelangfc\
mkdir src\
cd src\
git clone -b noetic-devel https://github.com/ROBOTIS-GIT/DynamixelSDK.git \
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Framework.git \
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Framework-msgs.git \
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Math.git \
git clone https://github.com/ROBOTIS-GIT/ROBOTIS-Utility.git \
cd .. \
catkin_make \
source devel/setup.bash 

# Running SIM
roslaunch humanoid_gazebo humanoid_gazebo.launch \
roslaunch humanoid_manager humanoid_gazebo.launch

