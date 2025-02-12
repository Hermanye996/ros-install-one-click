[![ROS1 VERSION](https://img.shields.io/badge/ROS1-Noetic-green)](http://wiki.ros.org/noetic) &nbsp;
[![Ubuntu for ROS1](https://img.shields.io/badge/Ubuntu-20.04-green)](https://ubuntu.com/) &nbsp;
[![ROS2 VERSION](https://img.shields.io/badge/ROS2-Humble-brightgreen)](http://docs.ros.org/en/humble/index.html) &nbsp;
[![Ubuntu_for_ROS2](https://img.shields.io/badge/Ubuntu-22.04-brightgreen)](https://ubuntu.com/) &nbsp;
[![LICENSE](https://img.shields.io/badge/license-Apache--2.0-informational)](https://github.com/mangdangroboticsclub/gpt4_ros2/blob/main/LICENSE) &nbsp;

# ros-install-one-click

This is a collection of one-click shell scripts for installing and using common tools for robotics, including ROS1, ROS2, camera, MoveIt, and simulators.

With these scripts, you can install ROS and other tools with one click, and then use robot tools conveniently with the help of the scripts.

## ROS 1 Noetic Installation

To install `ROS1 Noetic` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/ros1_noetic_install.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/ros1_noetic_install.sh && sudo chmod +x $HOME/ros1_noetic_install.sh && sudo bash $HOME/ros1_noetic_install.sh && rm $HOME/ros1_noetic_install.sh
```

## ROS 2 Humble Installation

To install `ROS2 Humble` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/ros2_humble_install.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/ros2_humble_install.sh && sudo chmod +x $HOME/ros2_humble_install.sh && bash $HOME/ros2_humble_install.sh && rm $HOME/ros2_humble_install.sh
```

## MoveIt 1 Installation

To install `MoveIt for ROS1 Noetic` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/moveit1_install.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/moveit1_install.sh && sudo chmod +x $HOME/moveit1_install.sh && sudo bash $HOME/moveit1_install.sh && rm $HOME/moveit1_install.sh
```

## Intel realsense D400 series camera Installation

To install `realsense D400 series camera` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/realsense_d400_series_install.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/realsense_d400_series_install.sh && sudo chmod +x $HOME/realsense_d400_series_install.sh && bash $HOME/realsense_d400_series_install.sh
```

To install `Realsense for Nvidia Jetson Orin` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/realsense_install_nvidia.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/realsense_install_nvidia.sh && sudo chmod +x $HOME/realsense_install_nvidia.sh && bash $HOME/realsense_install_nvidia.sh && rm $HOME/realsense_install_nvidia.sh
```

## Orbbec Femto Bolt Installation

To install `Orbbec Femto Bolt Camera ROS1 Noetic version` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/orbbec_femto_bolt_ros1_install.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/orbbec_femto_bolt_ros1_install.sh && sudo chmod +x $HOME/orbbec_femto_bolt_ros1_install.sh && bash $HOME/orbbec_femto_bolt_ros1_install.sh && rm $HOME/orbbec_femto_bolt_ros1_install.sh
```

To install `Orbbec Femto Bolt Camera ROS2 Humble version` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/orbbec_femto_bolt_ros2_install.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/orbbec_femto_bolt_ros2_install.sh && sudo chmod +x $HOME/orbbec_femto_bolt_ros2_install.sh && bash $HOME/orbbec_femto_bolt_ros2_install.sh && rm $HOME/orbbec_femto_bolt_ros2_install.sh
```

### Microsoft Azure Kinect DK Installation

To install `Azure Kinect DK` with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/azure_kinect_dk_install.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/azure_kinect_dk_install.sh && sudo chmod +x $HOME/azure_kinect_dk_install.sh && bash $HOME/azure_kinect_dk_install.sh
```

### Isaac Sim python assistant

The `Isaac Sim python assistant` script facilitates the execution of an Isaac Sim standalone Python script provided by the user.

```bash
# Go to your isaac sim standalone python directory
cd <your_python_directory>
# Download the script
wget https://raw.githubusercontent.com/auromix/ros-install-one-click/main/isaacsim_python_assistant.sh
# Grant execute permission
chmod +x isaacsim_python_assistant.sh
```

```bash
# Go to your isaac sim standalone python directory
cd <your_python_directory>
# Run the script to launch your isaac sim standalone python file
./isaacsim_python_assistant.sh
```

### Config Static IP

This script provides a command-line method to configure a static IP address for an Ethernet interface on a robot. It is particularly useful when a graphical user interface (GUI) is not easily accessible or feasible.

```bash
./config_static_ip.sh
```

### Config SSH for github

This script provides a command-line method to configure SSH for github.

```bash
script_name="config_ssh.sh" && directory_name="/tmp" && full_script_path="${directory_name}/${script_name}" && wget -O $full_script_path https://raw.githubusercontent.com/auromix/ros-install-one-click/main/$script_name && sudo chmod +x $full_script_path && bash $full_script_path && rm -rf $full_script_path
```

### Config VPN SSH Port

If you are using a VPN on router and need to access GitHub via SSH, you will likely need to reconfigure the SSH port.

```bash
./ config_vpn_ssh_port.sh
```

### Improve Jetson performance

To install the best performance setup and basic development environment for NVIDIA Jetson AGX Orin with a single command, copy and execute the following command in the terminal:

```bash
wget -O $HOME/jetson_best_performance_install_v512.sh https://raw.githubusercontent.com/auromix/ros-install-one-click/main/jetson_best_performance_install_v512.sh && sudo chmod +x $HOME/jetson_best_performance_install_v512.sh && bash $HOME/jetson_best_performance_install_v512.sh
```

### Config UDev Rules
The config_udev_rules.sh script simplifies the creation of udev rules to assign persistent, user-friendly names (symlinks) to devices connected to your system. It guides you through identifying new devices, extracting udev information, and generating a custom rule to ensure consistent device naming.
```bash
script_name="config_udev_rules.sh" && directory_name="/tmp" && full_script_path="${directory_name}/${script_name}" && wget -O $full_script_path https://raw.githubusercontent.com/auromix/ros-install-one-click/main/$script_name && sudo chmod +x $full_script_path && sudo bash $full_script_path && rm -rf $full_script_path
```

### Config CUDA

Run the script to configure your CUDA after CUDA installation.
```bash
script_name="config_cuda.sh" && directory_name="/tmp" && download_url="https://raw.githubusercontent.com/auromix/ros-install-one-click/main" && full_script_path="${directory_name}/${script_name}" && wget -O $full_script_path $download_url/$script_name && sudo chmod +x $full_script_path && bash $full_script_path && rm -rf $full_script_path
```
### Test CUDA and Torch

This script test your CUDA and Pytorch environment.

```bash
wget https://raw.githubusercontent.com/auromix/ros-install-one-click/main/test_cuda.py && python3 test_cuda.py
```

### Config Vs Code for Isaac Sim dev

Run the script in the top-level directory of your workspace to set up the Isaac Sim environment for VS Code, enabling the IDE to recognize the Isaac Sim package.
```bash
script_name="setup_isaac_sim_ide_environment.sh" && directory_name="/tmp" && download_url="https://raw.githubusercontent.com/Auromix/auro_sim/main/scripts" && full_script_path="${directory_name}/${script_name}" && wget -O $full_script_path $download_url/$script_name && sudo chmod +x $full_script_path && bash $full_script_path && rm -rf $full_script_path
```

