# ros_joycon_rlds 用法

## 准备工作

在正常能操控xarm的基础上安装两个repo

1. 遥控器控制以及适应仓库：https://github.com/box2ai-robotics/joycon-robotics。

2. Lerobot正逆运动学仓库：除了正逆运动学函数外，还包括键盘和Joycon控制仿真Mujoco和实物机器人的代码。另外还有一个完整的基于Genesis做双臂实例。https://github.com/box2ai-robotics/lerobot-kinematics。

Note： 需要使用被我们修改过的版本，不要直接clone原版。修改过的仓库在`./src/xarm_sys/scripts/xarm_joycon/joyconrobotics`和`/src/xarm_sys/scripts/xarm_joycon/lerobot_kinematics`

## 使用

运行`.ros_joycon_rlds/src/xarm_sys/scripts/xarm_joycon/run_all_nodes.sh`

## 其他说明

在林涛原有的代码上修改了`./ros_joycon_rlds/src/xarm_sys/scripts/xarm_joycon/examples/lerobot_joycon_gpos_xarm6_new.py`和`./ros_joycon_rlds/src/xarm_sys/scripts/xarm_joycon/joyconrobotics/joyconrobotics/joyconrobotics.py`两个文件。在原先的joycon控制基础上增加了手腕旋转控制相关功能。

