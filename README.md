# traversability_projection_ws

### Building with catkin
```bash
$ git clone --recursive https://github.com/ganlumomo/traversability_projection_ws.git
$ cd traversability_projection_ws/src/any_node
$ rm -rf any_node any_node_example any_worker signal_handler
$ catkin_make -DCMAKE_BUILD_TYPE=Release
```

### Running
```bash
$ roslaunch elevation_mapping_demos kitti.launch
$ roslaunch traversability_estimation kitti.launch
$ rosrun traversability_projection traversability_projection_node
$ rosrun kitti_player_mini kitti_player_mini_node
```
