# Action Server Client C++ Implementation

## CMakeLists.txt file modifications

Open session3_action/CMakeLists.txt and add following lines to the bottom of the file.

```sh
add_executable(server src/server.cpp)
target_link_libraries(server ${catkin_LIBRARIES})
add_dependencies(server ${actionlib_tutorials_EXPORTED_TARGETS}


add_executable(ac_client src/ac_client.cpp)
target_link_libraries(ac_client ${catkin_LIBRARIES})
add_dependencies(ac_client ${actionlib_tutorials_EXPORTED_TARGETS})
```

## Build the code 

Go to root of the workspace

```sh
cd ~/ros_workshop/
```
```sh
catkin build
```
or
```sh
catkin_make
```

## Run the code

Open a terminal and run,

```sh
roscore
```

Open a 2nd terminal in the workspace root and run,
	
```sh
source devel/setup.bash
```
```sh
rosrun session3_action server
```

Open a 3rd terminal in the workspace root and run,

```sh
source devel/setup.bash
```
```sh
rosrun session3_action ac_client
```

