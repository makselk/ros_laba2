# SLAM laba

## Запуск

- Установить зависимости:

``sudo apt-get install ros-noetic-joy ros-noetic-teleop-twist-joy \
  ros-noetic-teleop-twist-keyboard ros-noetic-laser-proc \
  ros-noetic-rgbd-launch ros-noetic-depthimage-to-laserscan \
  ros-noetic-rosserial-arduino ros-noetic-rosserial-python \
  ros-noetic-rosserial-server ros-noetic-rosserial-client \
  ros-noetic-rosserial-msgs ros-noetic-amcl ros-noetic-map-server \
  ros-noetic-move-base ros-noetic-urdf ros-noetic-xacro \
  ros-noetic-compressed-image-transport ros-noetic-rqt* \
  ros-noetic-gmapping ros-noetic-navigation ros-noetic-interactive-markers``

``sudo apt-get install ros-noetic-dynamixel-sdk``

``sudo apt-get install ros-noetic-turtlebot3-msgs``

``sudo apt-get install ros-noetic-turtlebot3``


- Клонировать репозиторий
``git clone https://github.com/makselk/ros_laba2.git ``

- Собрать это дело
``cd ros_laba2``
``catkin_make``
``source devel/setup.bash``

- Запустить при помощи .launch файла
``export TURTLEBOT3_MODEL=waffle_pi``
``roslaunch custom_pipeline custom_full.launch``

- Смотрим, как оно работает, показывая точку назначения при помощи "2D nav goal"

## Дополнительные параметры 'custom_full.launch'

- ``model`` - можно указать другую модель робота
- ``x_pos, y_pos, z_pos`` - начальное положение робота
- ``world`` - можно изменить модель мира на любую другую
