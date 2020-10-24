# Robotics_seminar
Instructions to setup your computer for the second session of the robotics webinar series

# ROS Noetic Installation

Setup your computer to accept ROS related software

```sh
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

Then setup keys

```sh
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```

To install ROS, 

```sh
sudo apt update
```

```sh
sudo apt install ros-noetic-desktop-full
```

Setup environment

```sh
echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
```

```sh
source ~/.bashrc
```

Dependencies

```sh
sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
```

```sh
sudo rosdep init
```

```sh
rosdep update
```

To setup catkin tools
```sh
pip3 install catkin_tools
```


Setup VS code as text editor

# ROS Melodic Installation

Setup your computer to accept ROS related software

```sh
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

Then setup keys

```sh
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```

To install ROS, 

```sh
sudo apt update
```

```sh
sudo apt install ros-melodic-desktop-full
```

Setup environment

```sh
echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
```

```sh
source ~/.bashrc
```

Dependencies

```sh
sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
```

```sh
sudo rosdep init
```

```sh
rosdep update
```

To setup catkin tools
```sh
pip3 install catkin_tools
```

Setup VS code as text editor

# ROS Kinetic Installation

Setup your computer to accept ROS related software

```sh
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

Then setup keys

```sh
sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```

To install ROS, 

```sh
sudo apt update
```

```sh
sudo apt-get install ros-kinetic-desktop-full
```

Setup environment

```sh
echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
```

```sh
source ~/.bashrc
```

Dependencies

```sh
sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
```

```sh
sudo rosdep init
```

```sh
rosdep update
```

To setup catkin tools
```sh
pip3 install catkin_tools
```


Setup VS code as text editor
