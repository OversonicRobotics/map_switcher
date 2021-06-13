# map_switcher

ROS package to switch between occupancy grid maps. Based on the ideas proposed by [multi_map_navigation](https://github.com/MohitShridhar/multi_map_navigation), but slimmed down to focus only on switching individual occupancy grids, without the navigation or elevator components.

# Execution Procedure

```
roslaunch map_switcher map_switcher.launch
```

Either of the following commands will switch the map
```
rosservice call /map_switcher/change_map elevator_1 map_floor0
```
```
rosservice call /map_switcher/change_map elevator_1 map_floor
```
