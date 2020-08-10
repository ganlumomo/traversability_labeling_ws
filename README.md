# traversability_projection_ws

### Building with catkin
```bash
$ git clone --recursive https://github.com/ganlumomo/traversability_projection_ws.git
$ cd traversability_projection_ws/src/any_node
$ rm -rf any_node any_node_example any_worker signal_handler
$ cd ../../
$ vim src/kindr_ros/kindr_rviz_plugins/include/kindr_rviz_plugins/VectorAtPositionDisplay.hpp
add #include <OgreMeshManager.h> in the header file
$ catkin_make -DCMAKE_BUILD_TYPE=Release
```

### Running
```bash
$ roslaunch elevation_mapping_demos kitti.launch
$ roslaunch traversability_estimation kitti.launch
$ rosrun traversability_projection traversability_projection_node
$ rosrun kitti_player_mini kitti_player_mini_node
```
