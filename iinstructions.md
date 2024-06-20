__Open a new terminal and source ROS 2 again.__

source /opt/ros/humble/setup.bash

echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc

(чтобы команду не вводить при запуске консоли)

At this point you should have three windows open: a terminal ()running turtlesim_node, 
a terminal running turtle_teleop_key and the turtlesim window. 

__ПРИМЕРЫ__

__ros2 run turtlesim turtle_teleop_key__

(teleop_turtle)

__ros2 run turtlesim turtlesim_node__

(имя turtlesim)

turtle_teleop_key active so that you can control the turtle in turtlesim.

__ros2 run <package_name> <executable_name>__

__ros2 node list__

- показывает работающие ноды
- -t с типами данных
  
  
__ros2 run turtlesim turtlesim_node --ros-args --remap __node:=my_turtle__

(создание нода моячерепаха)


__ros2 node info <node_name>__

__rqt_graph__

график как связаны ноды


__ros2 topic echo <topic_name>__

инфа, как двигается по осям xyz угловой и линейный


__ros2 topic info /turtle1/cmd_vel__

инфа про пб сб и тип


__ros2 interface show <msg type>__

показывает, какой тип ожидает топик(из примера шест значений угловой-линейный xyz)


__ros2 topic pub <topic_name> <msg_type> '<args>'__

структура сообщения




