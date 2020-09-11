# 3D-Classroom-using-OpenGL

### Desciption:
This project aims to create a 3D Model of a classroom in openGL. The classroom consists of various objects such as table, chair, blackboard, windows, door etc.
We can navigate through the classroom using a mouse and a keyboard. The mouse is used to rotate around the current position, whereas the keyboard is used to move around the classroom.
We have added animation to the fan which makes the fan rotate continuously. “Welcome” Text was inserted near the snowman at the window making it appear as if it greets the visitor near him.

### Library Used:
Along with OpenGL, the library GLUT was used to create the window and set the projection and configure the camera. GLUT handles the 3D pipelining which consists of normalizing, clipping, projection( perspective ) and transformation to viewport coordinates.

### Header Files:
Header files contain definitions of Functions and Variables, which is imported or used into any C++ program by using the pre-processor #include statements. The list of user defined header files are:
chair.h : 
This header file contains a class with the method necessary to draw a chair.
cupboard.h :
This header file contains a class with the method necessary to draw a cupboard.
fan.h :
This header file contains a class with the method necessary to draw a fan and animate it by changing the angle of rotation.
shelf.h :
This header file contains a class with the method necessary to draw a shelf and the items placed inside it.
snowman.h :
This header file contains a class with the method necessary to draw a snowman.
table.h :
This header file contains a class with the method necessary to draw a table.
window.h :
This header file contains a class with the method necessary to draw window and window sill.

### Classroom:
classroom.cpp creates the 3D environment. It makes use of the different header files to add the objects to the classroom by applying translation, rotation and scaling.
It also defines the callback functions to handle the keyboard and mouse events. These events trigger the movement and rotation of the camera. Thus, providing a first-person experience of a 3D classroom .

Mouse : This is used to look around the classroom from the current position.
Keyboard: This is used to move around the classroom and rotate the viewing angle.
	The list of keyboard commands are:
W or UP arrow : move forward
S or DOWN arrow : move backward
A or LEFT arrow : move left
D or RIGHT arrow : move right
Z : roll left
X : roll right 

Description of classroom :
  A door is inserted at the rear wall of the classroom. We start from outside the classroom and can enter it by this door.
  The front wall has a blackboard on it. 
  In the front of the blackboard is Teacher’s table and chair placed at the right of the blackboard at a certain angle.
  There are 16 sets of student tables and chairs in front of the blackboard .
  Along the right wall, there is a purple cupboard.
  On the right wall, beside the cupboard, there are two shelves at different heights  joined at a single vertex. The top shelf has three snowmen colored red, white and yellow.
  The left wall has two windows at the same horizontal height with a small ledge at the bottom of each.
  The window closer to the blackboard has a white snowman on its ledge. A message “Welcome” is visible near the snowman.
  The ceiling has a fan that keeps rotating.
  
### Prerequisite:
Installing  openGL 
      Enter the following commands in the terminal:
    $ sudo apt update

   $ sudo apt-get install freeglut3 freeglut3-dev

   $ sudo apt-get install binutils-gold

   $sudo apt-get install mesa-utils
 
        
### How to Run:
  To run the 3D-classroom, Open the terminal in directory containing the program classroom.cpp(CS_352_project/3D-Classroom/) and then run the following commands:

   $ cmake . 
   $ make all				//creates an output file named Classroom 
   $ ./Classroom 			//run the output file

   $ make clean 			//removes all object file that was created

      
  
  
  
 This minor project was done as part of Computer Graphics course in B.Tech CSE, with the help of my project member https://github.com/vkumar7796
