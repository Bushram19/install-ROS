# install-ROS
I downloaded the VM and Ubuntu version 20.04.
I visited the website "http://wiki.ros.org/noetic/Installation/Ubuntu" to follow the steps to install ROS.
steps :
1-Installation.
2-Configure my Ubuntu repositories.
3-Setup your sources.list , Setup your computer to accept software from packages.ros.org. code "sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'"
4-Set up my keys , code "sudo apt install curl # if you haven't already installed curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -"
5-the Installation First, make sure your Debian package index is up-to-date:code "sudo apt update"
6-Now choose how much ROS you want to install:full 
Desktop-Full Install: (Recommended) : Everything in Desktop plus 2D/3D simulators and 2D/3D perception packages,code "sudo apt install ros-noetic-desktop-full"
7-We prepare the environment , code"source /opt/ros/noetic/setup.bash"
Bash "echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc source ~/.bashrc"
zsh "echo "source /opt/ros/noetic/setup.zsh" >> ~/.zshrc source ~/.zshrc"
8-Dependencies for building packages : Up to now you have installed what you need to run the core ROS packages.
To install this tool and other dependencies for building ROS packages, run: code "sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential"
finally,Initialize rosdep :code "sudo apt install python3-rosdep"
With the following, you can initialize rosdep, code "sudo rosdep init" , "rosdep update" 
ROS system installed successfully.
