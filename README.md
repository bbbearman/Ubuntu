[**ROS Wiki (cn)**](http://wiki.ros.org/cn/ROS/Tutorials)
******
## Create Workspace
```bash
mkdir -p catkin_ws/src
cd catkin_ws/src
#catkin_make

git clone [package]
catkin_init_workspace

cd .. #back to your workspace
catkin build

source devel/setup.bash
```
******
## ROS Command

`rosnode list` show the nodes that run in ros
`rosnode info/nodes`

**TOPIC**  Publisher and Subscriber
`rostopic echo [topic]` 显示话题上的数据
`rostopic type [topic]`
`rostopic pub [topic] [msg_type] -r 1 -- [args]`
`rostopic hz [topic]`  报告发送速率

`rosrun rqt_plot rqt_plot` 回执被发布到话题上的数据

**SERVICE** Server and Client
`rosservice type [service]`
`rosservice call [service] [args]`
`rosparam set` etc...
******

