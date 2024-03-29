# URDF to DH Parameterization

v0.0.1

Sometimes people want DH... ```¯\_(ツ)_/¯```

## Documentation

Check out the [documentation](https://mcevoyandy.github.io/urdf_to_dh/index.html) for more details on how the conversion is done and how to use this package.

## Installation:
```
pip3 install anytree
pip3 install pandas
pip3 install tabulate
```

## Create a workspace, build and source:
```
mkdir urdf_to_dh_ws
cd urdf_to_dh_ws
mkdir src
cd src
git clone https://github.com/mehmet-engineer/ros2_urdf_to_dh_parameters
cd ..
colcon build
source install/setup.bash
```

## Running the node

```
ros2 run urdf_to_dh generate_dh --ros-args -p urdf_file:="<path_to_my_urdf>"
```

**雙臂8軸**
- **☀timda_dual8☀ TIMDA雙臂(滑軌可動)**
    urdf_file:="/home/iclab/work/manip_metrics/src/manipulability_metrics_examples/urdf/timda_dual8.xacro"

**雙臂7軸**

- **☀timda_dual7☀ TIMDA雙臂(滑軌固定)** 
    urdf_file:="/home/iclab/work/manip_metrics/src/manipulability_metrics_examples/urdf/timda_dual7.xacro"
    

**單臂8軸**

- **☀timda_single8☀ TIMDA單臂(滑軌可動)**
    urdf_file:="/home/iclab/work/manip_metrics/src/manipulability_metrics_examples/urdf/timda_single8.xacro"

**單臂7軸**

- **☀timda_single7☀ TIMDA單臂(滑軌固定)** 
    urdf_file:="/home/iclab/work/manip_metrics/src/manipulability_metrics_examples/urdf/timda_single7.xacro"
    urdf_file:="/home/iclab/work/manip_metrics/src/robot_models/timda/single_arm_description/urdf/single_arm.urdf.xacro"


- **☀blue_arm☀ 藍色小手臂** 
    urdf_file:="/home/iclab/work/manip_metrics/src/robot_models/blue_arm_description/urdf/blue_arm.xacro"
    
- **☀kuka_iiwa☀ KUKA LBR IIWA 7 R800**
    urdf_file:="/home/iclab/work/manip_metrics/src/robot_models/iiwa_description/urdf/iiwa7.urdf.xacro"

**單臂6軸**

- **☀ur5☀ UR5**
    urdf_file:="/home/iclab/work/manip_metrics/src/robot_models/ur_description/urdf/ur.urdf.xacro name:=ur5"
    urdf_file:="/home/iclab/work/manip_metrics/src/robot_models/ur_description/urdf/ur5.urdf.xacro"

- **☀ur5e☀ UR5e**
    urdf_file:="/home/iclab/work/manip_metrics/src/robot_models/ur_description/urdf/ur.urdf.xacro name:=ur5e"

- **☀kuka_kr6☀ KUKA KR6 R900 Sixx**
    urdf_file:="/home/iclab/work/manip_metrics/src/robot_models/kuka_kr6_support/urdf/kr6r900sixx.xacro"