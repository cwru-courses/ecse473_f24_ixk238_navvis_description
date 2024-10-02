# ECSE473 Modern Robotic Programming Laboratory 2

The project directory structure is in this way as mentioned in Laboratory description:

```
  navvis_description
  ├── CMakeLists.txt
  ├── package.xml
  ├── launch
  │   ├── display.launch 
  ├── config
  │   └── config.rviz
  ├── urdf
  │   ├── robot.urdf
  │   └── robot.xacro
  └── README.md
```
### Prerequisites

In order to launch the project, you should already have:
- Installed ROS Noetic
- The joint state publisher GUI
  ```
  
    sudo apt install ros-noetic-joint-state-publisher-gui
  
  ```
- Gazebo plugins
  ```
  
    sudo apt install ros-noetic-plugins
  
  ```
- Velodyne description
  ```
  
    sudo apt install ros-noetic-velodyne-description
  
  ```
### Available Parameters to use with display.launch

The launch file takes three arguments:
-  use_xacro:=(true|false) - whether the xacro file will be used to launch 
-  file - file name
-  use_joint_state_publisher_gui=(true|false)  whether the joint_state_publisher_gui will be used 

### View the Robot Description in rviz

- #### rviz with the joint_state_publisher GUI

  - ##### Launch by using the urdf file

  ```

    roslaunch navvis_description display.launch

  ```
  - ##### Launch by using the xacro file

  ```

    roslaunch navvis_description display.launch use_xacro:=true

  ```
- #### rviz with the joint_state_publisher GUI

  - ##### Launch by using the urdf file

  ```

    roslaunch navvis_description display.launch use_joint_state_publisher_gui:=false

  ```

  - ##### Launch by using the xacro file

  ```

    roslaunch navvis_description display.launch use_xacro:=true use_joint_state_publisher_gui:=false

  ```
## Authors

  - **Ilke Kas** - *PhD at ECSE* -
    [Ilke Kas Github](https://github.com/ilke-kas)

