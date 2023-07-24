# 功能介绍

创建自己的第一个Node。控制turtlesim做绕圈运动

# 物料清单

以下机器人均已适配RDK X3
| 物料选项    | 清单      | 
| ------- | ------------ |
| 机器人名称          | 生产厂家 | 参考链接                                        |
| RDK X3 Robot        | 多厂家 | [点击跳转](https://developer.horizon.ai/sunrise) |

# 使用方式

## 准备工作

1. RDK X3 使用desktop版本，能够正常访问互联网

## 安装first-node功能包

启动机器人后，通过终端或者VNC连接机器人，点击右上方的“一键部署”按钮，复制命令在RDK的系统上运行，完成hobot-nav2功能包的安装。

```bash
sudo apt update
sudo apt install -y tros-first-node
```

## 运行first-node功能包

通过MoBaXterm连接机器人，启动命令如下：

```bash
# 设置tros的环境变量
source /opt/tros/setup.bash

# 启动Turtlesim
ros2 run turtlesim turtlesim_node
```

再另一个终端中启动firs_node

```bash
# 设置tros的环境变量
source /opt/tros/setup.bash

# 启动OriginBot
ros2 run first_node first_node
```

## 使用键盘控制turtlesim

通过MoBaXterm连接机器人，启动命令如下：

```bash
# 设置tros的环境变量
source /opt/tros/setup.bash

# 启动Turtlesim
ros2 run turtlesim turtlesim_node
```

再另一个终端中启动turtle_teleop_key

```bash
# 设置tros的环境变量
source /opt/tros/setup.bash

# 启动OriginBot
 ros2 run turtlesim turtle_teleop_key
```

根据提示使用键盘“上、下、左、右”按钮控制turtlesim移动

# 接口说明

## 发布话题
| 名称         | 消息类型                             | 说明                                     |
| ------------ | ------------------------------------ | ---------------------------------------- |
| /turtle1/cmd_vel | geometry_msgs/msg/Twist           | turtlesim运动控制命令 |


# 参考资料

暂无


# 常见问题

暂无
