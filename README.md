# raspbot_v2_nav

## Описание ROS2 пакетов управления роботом
Проект содержит ROS2-пакеты для управления Yahboom роботом, включая пакеты для управления шасси, визуализации, управления с клавиатуры и описания робота в URDF.

### Пакеты ROS2 в `thirdparty/ros2_ws/src`
- [yahboomcar_bringup](thirdparty/ros2_ws/src/yahboomcar_bringup/README.md) — драйвер шасси и запуск системного bringup для робота.
- [yahboomcar_ctrl](thirdparty/ros2_ws/src/yahboomcar_ctrl/README.md) — управление роботом с клавиатуры.
- [yahboomcar_description](thirdparty/ros2_ws/src/yahboomcar_description/README.md) — URDF/mesh-описание робота, запуск `robot_state_publisher` и визуализация в RViz.
- [yahboomcar_msgs](thirdparty/ros2_ws/src/yahboomcar_msgs/README.md) — собственные сообщения ROS2 для управления роботом.

