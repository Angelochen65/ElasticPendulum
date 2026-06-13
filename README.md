Web VPython 3.2
#Overview
#This is a physics simulation of springs in series that act as a pendulum. We were inspired by the physics behind a bungee rope,
#and how it acts as many different springs that are connected to one another. This is a simulation of how a rope acts when it is
#attatched at a single point and there is a mass at the end of the rope (modeled as a sphere shaped cow). 

#User Controls
#The aspects of the spring(s) that the user is able to control is the number of springs, the mass of the cow ball, the angle in
#the X-Y direction, the angle in the Z direction, and the length of the spring. The user can change these controls through sliders. 
#The default mode for simulation is one spring, a 50 kilogram cow, a spring length of 2 centimeters, and initial XY and Z angles of 0. 
#For the XY and Z sliders, the user can move the slider node left to move the spring to the left/back and then can move the node right
#to move the spring right/forward.

#Animation
#Once the user choose each aspect of the spring simulation, the simulation begins when the red Start button is pressed. Once the button is
#pressed, the animation begins. The user can choose to stop the simulation and change different parts of the spring by pressing the red button
#once more (which should say "Stop"), and resume the animation by pressing the red button again. To reset the whole simulation and go back
#to the default values and camera setting, the user can press the blue Reset button. To trace the path of the cow, the user can press
#the Toggle Trace button to turn the trace on and off. The default is for the trace to be off, but once the simulation begins, the
#user can turn on the traced path. When the trace is turned off during the animation, the previous path is cleared and there is no
#more traced path. During the simulation, the user is able to move around the camera and perspective with a computer mouse/pad. However,
#once the reset button is pressed, the camera is reset to face the spring. 
#The animation was made using the Euler-Cromer Method, where the physics of the spring is shown through small increments of time. Each
#spring is affected by a gravitational force and a spring force. If there are multiple springs in the simulation, the net force is determined
#by the previous spring's position and spring force. 

#Graphs
#Once the start button is pressed, there will be two different graphs that are below the control sliders. There is an energy graph, 
#which plots the gravitational potential energy of the cow ball in green, the total elastic potential energy of the spring(s) in red,
#and the kinetic energy of the cow in blue. The graph is Time (s) vs. Energy (J). There is also a phase graph, which plots the cow ball's
#velocity against the cow ball's position. There is a curve for the x, y, and z components of the velocity and position, where the
#x component is orange, the y component is purple, and the z component is cyan. 
