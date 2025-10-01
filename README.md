# Yahboom робот с mecanum колесами #
 
This package contains mobile robot navigation fot yahboom robot.
 
## Description
 
The package includes ROS 2 code for yahboom robot navigation 
 
## Prerequisites
 
- ROS 2 must be installed
- Python 3
- Created ROS 2 workspace (`ros2_ws`)
 
## Author
 
Larionov Alex


## How to run 


1. Клонируйте репозиторий и скопируйте папку yahboom_rosmaster в ваш ROS2 Workspace.

2. Запустите, чтобы собрать ros пакет :

cd ~/ros2_ws/ && colcon build && source ~/.bashrc

3. Обновить:

sudo apt update -y && sudo apt upgrade -y

4. Обновите установленные пакеты: 

rosdep install --from-paths src --ignore-src -r -y

5. Запустите скрипт для полного запуска конфигураций робота и окружения:

bash ~/ros2_ws/src/yahboom_rosmaster/yahboom_rosmaster_bringup/scripts/rosmaster_x3_navigation.sh

6. Запустите скрипт, чтобы тележка двигалась по квадрату

ros2 run yahboom_rosmaster_system_tests square_mecanum_controller 
