# TEAM 4

##  ASSIGNMENT 3   


## Navigating through assignment 3:

'''

				    | -> worlds --> turtlebot3_wall.world
				    | 
			 |--> src --| -> launch --> move.launch
			 |	    |           --> emergency_brake_wall.launch
			 | 	    | 
			 |	    |              | --> circle.py
Assignment3_turtlebot3- |          | -> scripts --|--> square.py
			 |			    | --> emergency_braking.py
			 |
			 |
			 | 	       |--> emergency braking.webm
			-|--> videos --|--> circle.webm
			               |--> square.webm
'''
			

In Assignment 3 we have 2 tasks

Task 1
	A) Move the turtlebot in circular motion.
		We use the python script circle.py for its implementation.It uses the
		concept that when given a same angular and linear velocity to the 
		bot it moves in circular motion.
		
		Use Command
	''' $ roslaunch assignment3_turtlebot3 move.launch code:=circle '''
	
	
	
	B) Move the turtlebot in a square motion.
		We use the python script square.py for its implementation. It uses
		three while loops the first one tells that there are four similar
		motion ie. straight motion and 90 deg rotation. We used 0.2 linear and
		angular velocity to reduce the error in gazebo and also some gain 
		added to the rotation by trial and error to have a trajectory similar
		to square.
		
		Use command
       ''' $ roslaunch assignment3_turtlebot3 move.launch code:=square '''
	
	
	
	Launch File
		We create one launch file to open our world in gazebo and the two
		abovementioned nodes ie. circle and square motion.
		


Task 2:
	In task 2 we create a world with the turtlebot3 and a wall. Then we simulate
	a script called emergency_braking.py which moves the turtlebot3 in a straight
	motion but stops at emergency distance from the wall after it senses the wall.
	
	Use command
  ''' $ roslaunch assignment3_turtlebot3 emergency_brake_wall.launch '''
  
  
	Launch File:
		We create this launch file which opens the world with the wall and 
		turtlebot in gazebo and the executes the python script (node) 
		emergency_braking.py
		
	
	
		 	  
 
