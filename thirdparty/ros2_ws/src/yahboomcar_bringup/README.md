# yahboomcar_bringup

## Описание
ROS 2 пакет для инициализации аппаратной части робота и запуска драйвера шасси.

## Запускаемые узлы
- `Mcnamu_driver` — console script `yahboomcar_bringup.Mcnamu_driver:main`

## Launch файлы
- `launch/bringup.launch.py`
  - запускает `Mcnamu_driver`
- `launch/yahboomcar_bringup.launch.py`
  - запускает `Mcnamu_driver`
  - включает launch-файл `yahboomcar_description/launch/description_launch.py`

## Примеры запуска
- `ros2 launch yahboomcar_bringup bringup.launch.py`
- `ros2 launch yahboomcar_bringup yahboomcar_bringup.launch.py`
- `ros2 run yahboomcar_bringup Mcnamu_driver`

## Зависимости
- `rclcpp`
- `std_msgs`
- `yahboomcar_description` (через launch include)

## Структура
- `package.xml`
- `setup.py`
- `launch/bringup.launch.py`
- `launch/yahboomcar_bringup.launch.py`
- `yahboomcar_bringup/Mcnamu_driver.py`
