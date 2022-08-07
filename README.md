# Download Ros
## step1
***1- Download Oracle VM VirtualBox***
## step2
***2- Downlod ubuntu 20.04.2 Ubuntu 20.04.2 Desktop.iso***

***3- Start ubuntu linux installation***

***4-Restart and login***

## Step3
***5-Ubuntu desktop***

***6-Install Guest Additions***

***-open terminal***

```
### sudo apt-get update sudo apt-get upgrade 

### sudo apt install build-essential dkms linux-headers-$(uname -r) 
```
## Step4
Downlod ros 
```
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
sudo apt-get update
sudo apt-get install ros-kinetic-desktop-full
apt-cache search ros-kinetic
echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc source ~/.bashrc
sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
sudo apt install python-rosdep
sudo rosdep init
rosdep update
sudo apt-get install ros-noetic-catkin
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make
cd ~/catkin_ws/src
git clone https://github.com/smart-methods/arduino_robot_arm.git
cd ~/catkin_ws
rosdep install --from-paths src --ignore-src -r -y
sudo apt-get install ros-kinetic-moveit
sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui
sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher
sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control
sudo nano ~/.bashrc
at the end of the (bashrc) file add the follwing line source /home/HERE I BUT MY OWN NAME/catkin_ws/devel/setup.bash then ctrl + o
source ~/.bashrc
roslaunch robot_arm_pkg check_motors.launch
```
