# yahboomcar_description

## Описание
ROS 2 пакет, предоставляющий описание робота Yahboom Car (Raspbot V2) в виде URDF/химер и RViz-конфигураций.
Пакет содержит launch-файлы для публикации `robot_description`, запуска `joint_state_publisher` и визуализации модели в RViz.

## Launch файлы
- `launch/description_launch.py`
  - загружает URDF `urdf/Raspbot-V2.urdf`
  - запускает `robot_state_publisher`
  - запускает `joint_state_publisher`
  - запускает `static_transform_publisher` для `base_footprint` → `base_link`
- `launch/display_launch.py`
  - загружает URDF `urdf/Raspbot-V2.urdf`
  - запускает `robot_state_publisher`
  - запускает `joint_state_publisher_gui`
  - запускает `static_transform_publisher`
  - запускает `rviz2` с конфигурацией `rviz/raspbotv2.rviz`
- `launch/description_multi_robot1.launch.py`
  - загружает URDF `urdf/MicroROS_robot1.urdf`
  - запускает тот же стек узлов в namespace `robot1`
- `launch/description_multi_robot2.launch.py`
  - загружает URDF `urdf/MicroROS_robot2.urdf`
  - запускает тот же стек узлов в namespace `robot2`

## Файлы описания
- `urdf/Raspbot-V2.urdf`
- `urdf/Raspbot-V2.csv`
- `meshes/` — STL-модели звеньев и корпуса
- `rviz/raspbotv2.rviz`

## Примеры запуска
- `ros2 launch yahboomcar_description description_launch.py`
- `ros2 launch yahboomcar_description display_launch.py`
- `ros2 launch yahboomcar_description description_multi_robot1.launch.py`
- `ros2 launch yahboomcar_description description_multi_robot2.launch.py`

## Зависимости
- `robot_state_publisher`
- `joint_state_publisher`
- `joint_state_publisher_gui`
- `tf2_ros`
- `rviz2`
- `xacro`

## Структура
- `package.xml`
- `setup.py`
- `launch/`
- `urdf/`
- `meshes/`
- `rviz/`
- `resource/`
