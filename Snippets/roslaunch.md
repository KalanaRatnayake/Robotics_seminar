# ROSLAUNCH


## Syntax

```sh
<node pkg="evaluator" type="evaluator_node" name="evaluator" output="screen" />
```

<br>

## Sample launch file

```sh

<launch>
    <node pkg="session3_pubsub" type="publisher" name="publisher_1" output="screen" />
    <node pkg="session3_pubsub" type="publisher" name="publisher_2" output="screen" />
    <node pkg="session3_pubsub" type="subscriber" name="subscriber" output="screen" />
</launch>

```

## Use

Open a terminal and run,
	
```sh
source devel/setup.bash
```
```sh
roslaunch session3_pubsub test.launch
```