# Custom Action Creation

## Messages

Create a action folder inside session3_action folder

```sh
mkdir -p ~/ros_workspace/src/session3_action/action
```

Open the folder 
```sh
cd ~/ros_workspace/src/session3_action/action
```

Create a .action file with desired name. (we will select custom.action as an example)

```sh
code custom.action
```
Inside the file add following lines, then save and close.
```sh
uint8 start
---
uint8 finish
---
uint8 timeSpent
```

Open package.xml and add the following lines in the respective sections

```sh
<build_depend>actionlib_msgs</build_depend>
<build_export_depend>actionlib_msgs</build_export_depend>
<exec_depend>actionlib_msgs</exec_depend>
<exec_depend>message_generation</exec_depend>
```

Open the CMakeLists.txt and add following lines to respective section,

actionlib_msgs to find_package()

```sh
find_package(catkin REQUIRED COMPONENTS
   roscpp
   rospy
   std_msgs
   actionlib_msgs
)
```

actionlib_msgs to catkin_package

```sh
catkin_package(
  ...
  CATKIN_DEPENDS actionlib_msgs ...
  ...)
```

uncomment add_action_files section and add custom.action file

```sh
add_action_files(DIRECTORY 
  action
  FILES
  custom.action
)
)
```

uncomment generate_messgae() section and add actionlib_msgs. It shoul look like this,

```sh
generate_messages(
  DEPENDENCIES
  std_msgs
  actionlib_msgs
)
```