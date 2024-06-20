__Open a new terminal and source ROS 2 again.__
source /opt/ros/humble/setup.bash

echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc

(чтобы команду не вводить при запуске консоли)

At this point you should have three windows open: a terminal ()running turtlesim_node, 
a terminal running turtle_teleop_key and the turtlesim window. 

ПРИМЕРЫ

ros2 run turtlesim turtle_teleop_key

(teleop_turtle)

ros2 run turtlesim turtlesim_node 

(имя turtlesim)

turtle_teleop_key active so that you can control the turtle in turtlesim.

ros2 run <package_name> <executable_name>

ros2 node list

- показывает работающие ноды
- -t с типами данных
  
ros2 run turtlesim turtlesim_node --ros-args --remap __node:=my_turtle

(создание нода моячерепаха)

ros2 node info <node_name>

rqt_graph 

график как связаны ноды

ros2 topic echo <topic_name>

инфа, как двигается по осям xyz угловой и линейный

ros2 topic info /turtle1/cmd_vel

инфа про пб сб и тип

ros2 interface show <msg type>

показывает, какой тип ожидает топик(из примера шест значений угловой-линейный xyz)

ros2 topic pub <topic_name> <msg_type> '<args>'

структура сообщения




