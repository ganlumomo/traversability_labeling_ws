# traversability_projection_ws

### Building with catkin
```bash
$ git clone --recursive git@github.com:ganlumomo/traversability_projection_ws.git
$ cd traversability_projection_ws/src/any_node
$ rm -rf any_worker any_node any_node_example
$ cd ../../
$ catkin_make -DCMAKE_BUILD_TYPE=Release
```

### Troubleshooting
1. **Fatal error**: filters/filter_base.hpp: No such file or directory. **Solution**: For ROS Melodic, substitute each ```<filters/*.hpp>``` in grid_map package with ```<filters/*.h>```. See [https://github.com/ANYbotics/grid_map/issues/292](https://github.com/ANYbotics/grid_map/issues/292).

### Running
```bash
$ roslaunch elevation_mapping_demos kitti.launch
$ roslaunch traversability_estimation kitti.launch
$ rosrun traversability_projection traversability_projection_node
$ rosrun kitti_player_mini kitti_player_mini_node
```
