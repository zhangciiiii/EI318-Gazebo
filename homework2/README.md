# 作业二：SLAM导航


## 启动建图程序
打开新的终端，修改环境遍变量

```
TURTLEBOT_3D_SENSOR=AstraHokuyo
```

同一终端下运行，打开激光雷达建图程序

```
roslaunch robot_hokuyo_astra my_world_hk.launch
```

## 启动Rviz显示建图效果
打开一个新的控制终端，使用以下命令启动Rviz

```
roslaunch turtlebot_rviz_launchers view_navigation.launch
```

## 遥控机器人建图
打开一个新的控制终端启动仿真机器人平台键盘遥控 程序

```
roslaunch turtlebot_teleop keyboard_teleop.launch
```

保存建好的地图

```
mkdir ~/catkin_ws/src/turtlebot_learn/maps

rosrun map_server map_saver -f /home/mustar/catkin_ws/src/turtlebot_learn/maps/C1
```
