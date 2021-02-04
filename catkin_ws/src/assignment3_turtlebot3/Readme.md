# TEAM 4

##  ASSIGNMENT 3   


### Navigating through assignment 3:

![navigation](https://github.com/kloya03/AuE893_KartikLoya_Sp21/blob/master/catkin_ws/src/assignment3_turtlebot3/videos/navigation.png)	

In Assignment 3 we have 2 tasks:-

### Task 1

	A) Move the turtlebot in circular motion.
		We use the python script circle.py for its implementation.
		It uses the concept that when given a same angular and linear 
		velocity to the bot it moves in circular motion. Use the below 
		command to execute.
		
	
	B) Move the turtlebot in a square motion.
		We use the python script square.py for its implementation. 
		It uses three while loops the first one tells that there are 
		four similar motion ie. straight motion and 90 deg rotation. 
		We used 0.2 linear and angular velocity to reduce the error 
		in gazebo and also some gain added to the rotation by trial 
		and error to have a trajectory similar to square. Use the 
		below command to execute.
			
	
	Launch File
		We create one launch file to open our world in gazebo and the
		 two abovementioned nodes ie. circle and square motion.
		


### Task 2:

	C) Emergency braking when the turtlebot senses an object.
		In task 2 we create a world with the turtlebot3 and a wall.
		 Then we simulate a script called emergency_braking.py which 
		 moves the turtlebot3 in a straight motion but stops at 
		 emergency distance from the wall after it senses the wall.
		 Use the below command to execute.
	
  
	Launch File
		We create this launch file which opens the world with the 
		wall and turtlebot in gazebo and the executes the python 
		script (node) emergency_braking.py
		
		

A) '$ roslaunch assignment3_turtlebot3 move.launch code:=circle'  
 
B) '$ roslaunch assignment3_turtlebot3 move.launch code:=square'  

C) '$ roslaunch assignment3_turtlebot3 emergency_brake_wall.launch'   
		  
 
