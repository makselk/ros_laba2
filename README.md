# SLAM laba

## Запуск

- Клонировать репозиторий в catkin_ws
``git clone https://github.com/makselk/ros_laba2.git ``

- Собрать это дело
``catkin_make``
``source devel/setup.bash``

- Запустить при помощи .launch файла
``export TURTLEBOT3_MODEL=waffle_pi``
``roslaunch custom_pipeline custom_full.launch``

- Смотрим, как оно работает (через ж*пу), показывая точку назначения при помощи "2D nav goal"

## Дополнительные параметры 'custom_full.launch'

- ``model`` - можно указать другую модель робота
- ``x_pos, y_pos, z_pos`` - начальное положение робота
- ``world`` - можно изменить модель мира на любую другую
