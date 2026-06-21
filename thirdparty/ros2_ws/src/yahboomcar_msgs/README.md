# yahboomcar_msgs

## Описание
ROS 2 пакет с пользовательскими сообщениями для взаимодействия модулей робота.

## Описанные сообщения
- `ServoControl` — команда для управления сервоприводами
- `PointArray` — массив точек
- `Position` — простая позиция

## Зависимости
- `geometry_msgs`
- `std_msgs`
- `rosidl_default_generators`
- `rosidl_default_runtime`

## Команда сборки
- `colcon build --packages-select yahboomcar_msgs`

## Структура
- `package.xml`
- `CMakeLists.txt`
- `msg/ServoControl.msg`
- `msg/PointArray.msg`
- `msg/Position.msg`
