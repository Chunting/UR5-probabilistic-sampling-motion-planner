### UR5-probabilistic-sampling-motion-planner
This package enables us to use a sampling-based path planner to plan collision-free motions of a UR5 robot<br />
in ROS MoveIt! platform <br />

###How to use:
 Add Objects:<br />
First,  add objects to your scene.  In the \Scene Objects" tab,  click on \Import File".  A dialog <br />
window will allow you to search for 3D objects that you can import in your scene.  You can use <br />
your own objects or you can use the panel.dae provided in the directory assignment3/meshes <br />
(you can add the same object several times).  The object will appear green in the 3D view panel <br />
with an interactive marker.  Interactive markers have arrows and wheels that allow to translate and <br />
rotate the object by clicking and dragging them.  Move the object near the arm as illustrated in <br />
Fig.  3.  Once you are done select the Context tab, select the CS436 planning algorithm from the <br />
drop-down menu and click on the button Publish Current Scene <br /> <br />

Set a Goal Con guration:<br />
Now you need to define a goal configuration of the robot.  Notice that there is another interactive <br/>
marker at the wrist of the robot.  The marker enables you to move the end-effector of a robot to a <br/>
goal con guration by using the arrows and wheels of the marker.  Likewise, you can select a random <br />
valid goal state by clicking on the Update button on the Planning tab.  This will generate a valid <br />
(collision-free) random goal position of the robot and display the robot in orange.  You can change <br />
the position again by clicking on Update.<br />

 Plan the Motion: <br />
To plan the motion,  click on the Planning tab and click on the Plan button.  If the planner is successful,<br />
the robot will move from the start position to the goal position by avoiding the objects. If the planner <br />
fails to find a path, a Failed message will be displayed below the Plan and Execute button.  In this case<br />
you can try to plan again by clicking the Plan button or you can change the goal state or change the planning<br /> 
algorithm. <br />
Launch the planner using : roslaunch assignment3 planner.launch <br />

