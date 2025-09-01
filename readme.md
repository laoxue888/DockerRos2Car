
---

## 前言

本项目介绍一种基于**Unity3D**引擎的**SLAM**多传感器仿真平台，可模拟 **IMU、RGB-D相机、激光雷达**传感器数据输出，为SLAM算法提供**低成本、高可控性、可复现**的仿真测试环境。

![alt text](images/rgbd_lidar.gif)

video:
> - [2025-6-29:【开源】SLAM技术之FAST_LIO和FAST_LIO2算法复现](https://www.bilibili.com/video/BV158gfzPEea/?vd_source=3bf4271e80f39cfee030114782480463)
> - [2025-6-19：【开源】SLAM技术之Unity3D仿真激光雷达、RGBD相机、IMU传感器](https://www.bilibili.com/video/BV1twNxz1E7s/?vd_source=3bf4271e80f39cfee030114782480463)
> - [2025-4-1:【开源】实现在unity3d中仿真小车，还能用机器人开发框架ros2控制喔](https://www.bilibili.com/video/BV1CGZbY6ESv/?vd_source=3bf4271e80f39cfee030114782480463)

## 搭建开发环境

> - Unity:2023
> - Ubuntu:22.04
> - Ros2:humble

## 在window中安装Unity

先安装UnityHub，然后再安装Unity3D



[https://unity.cn/releases](https://unity.cn/releases)

## 开发环境

[配置开发环境](/docs/userguide/1.installation/1.installation.md)

## 运行测试

## Unity3D传感器数据获取测试

```shell
source install/setup.bash 
ros2 launch ros_tcp_endpoint endpoint.launch.py
```

```shell
source install/setup.bash
ros2 run topic_converter_python image_unconpressed
```

```shell
rviz2
```

# 参考：
> - [docker-ros2-unity-tcp-endpoint](https://github.com/frankjoshua/docker-ros2-unity-tcp-endpoint/tree/master)
> - [Robotics-Nav2-SLAM-Example](https://github.com/Unity-Technologies/Robotics-Nav2-SLAM-Example?tab=readme-ov-file)
> - [unity坐赛车游戏，简单三分钟了解一下](https://www.bilibili.com/video/BV1LU4y1o7re/?vd_source=3bf4271e80f39cfee030114782480463)
> - [How to Setup Unity and ROS2 in less than 5 minutes!](https://www.youtube.com/watch?v=1X6uzrvNwCk)
> - [ros2-for-unity](https://github.com/RobotecAI/ros2-for-unity)
> - [moveit2_yolobb_ws](https://github.com/laoxue888/moveit2_yolobb_ws)
> - [Unity-Robotics-Hub](https://github.com/Unity-Technologies/Unity-Robotics-Hub)
