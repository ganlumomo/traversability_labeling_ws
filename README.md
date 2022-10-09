# traversability_labeling_ws

### Building with catkin
```bash
$ git clone --recursive git@github.com:ganlumomo/traversability_labeling_ws.git
$ cd traversability_projection_ws/src/any_node
$ rm -rf any_worker any_node any_node_example
$ cd ../../
$ catkin_make -DCMAKE_BUILD_TYPE=Release
```

### Running
```bash
$ roslaunch elevation_mapping_demos kitti.launch
$ roslaunch traversability_estimation kitti.launch
$ rosrun traversability_projection traversability_projection_node
$ rosrun dataset_ros_player kitti_player_mini_node
```

### Running for MiniCheetah
```bash
$ roslaunch dataset_ros_player mini_cheetah.launch
$ roslaunch elevation_mapping_demos mini_cheetah.launch
$ roslaunch traversability_estimation mini_cheetah.launch
$ rosrun traversability_projection traversability_projection_node
```

### Generate data for MiniCheetah IRL project
```bashg
$ roslaunch dataset_ros_player mini_cheetah_irl.launch
$ roslaunch elevation_mapping_demos mini_cheetah_irl.launch
```
