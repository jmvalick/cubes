## Summary
This is a computer graphics project for learning transformations, skyboxes, heightmaps, texture mapping, and general OpenGL programming. 

### Instructions to run:
- Run this [Executable](./Project_1/Project_1.exe) <br>
or
- Watch this [Demonstration](./Results/Project1_demostration.mkv) instead

### Controls:

	W, A, S, D to move camera

			    No Modifier							Shift								Ctrl
	U 	Increase rotation rate in x-axis | Increase the scale in x-axis | Positive translation in the x-Axis
	J 	Decrease rotation rate in x-axis | Decrease the scale in x-axis | Negative translation in the x-Axis
	I 	Increase rotation rate in y-axis | Increase the scale in y-axis | Positive translation in the y-Axis
	K 	Decrease rotation rate in y-axis | Decrease the scale in y-axis | Negative translation in the y-Axis
	O 	Increase rotation rate in z-axis | Increase the scale in z-axis | Positive translation in the z-Axis
	L 	Decrease rotation rate in z-axis | Decrease the scale in z-axis | Negative translation in the z-Axis

## Code
- Source code can be found here: [Code](./Project_1/Sources/Project1.cpp)

- Headers can be found here: [Headers](./Project_1/Headers/)

- Since this was a class project. Most of this project is starter code. Below are all of the change and implementation made by me.

### Implementations made:
- Project_1.cpp
	- lines 24-36:
		- variables for transformations
	- lines 202-206:
		- skybox textures are loaded in
	- lines 270-282:
		- model transformations of boxes from the inputs
	- lines 291-395
		- 5 remaining walls of skybox are drawn
		- transformations are applied to orient the faces correctly
		- translations are applied to follow the camera so the skybox seems infinite 
	- lines 435-490:
		- added control inputs
- heightmap.hpp
	- lines 73-91:
		- height map "Draw" function is implemented
	- lines 120-185:
		- "make_vertex" function is implemented
		- "create_heightmap" function is implemented
		- "create_indices" function is implemented
		- "setup_heightmap" function is implemented

### Credit:
- lines 88-95 and 155-162:  
	- https://learnopengl.com/Guest-Articles/2021/Tessellation/Height-map 
	- helped with creating indices and using the glDrawElements to draw from array