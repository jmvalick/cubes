## Summary
This folder contains the Project 1 starter code. 

Contents:
	Headers
	camera.hpp
	heightmap.hpp
	Project1.hpp
	shader.hpp
	Media
	heightmaps
	skybox
	textures
	Shaders
	shader.frag
	shader.vert
	shader_SI_P2.vert
	Sources
	Project1.cpp
	Project_1.exe

How to run: navigate  Project1_Intermediate2_Valick_Jamin->Project_1->Project_1.exe

Controls:
	W, A, S, D to move camera

			    No Modifier							Shift							Ctrl
	U: Increase rotation rate in x-axis | Increase the scale in x-axis | Positive translation in the x-Axis
	J: Decrease rotation rate in x-axis | Decrease the scale in x-axis | Negative translation in the x-Axis
	I: Increase rotation rate in y-axis | Increase the scale in y-axis | Positive translation in the y-Axis
	K: Decrease rotation rate in y-axis | Decrease the scale in y-axis | Negative translation in the y-Axis
	O: Increase rotation rate in z-axis | Increase the scale in z-axis | Positive translation in the z-Axis
	L: Decrease rotation rate in z-axis | Decrease the scale in z-axis | Negative translation in the z-Axis

Moddifications:
	Project_1.cpp
		lines 24-36:
			variables for transformations
		lines 202-206:
			skybox textures are loaded in
		lines 270-282:
			model transformations of boxes from the inputs
		lines 291-395
			5 remaining walls of skybox are drawn
			transformations are applied to orient the faces correctly
			translations are applied to follow the camera so the skybox seems infinite 
		lines 435-490:
			added control inputs
	heightmap.hpp
		lines 73-91:
			height map "Draw" function is implemented
		lines 120-185:
			"make_vertex" function is implemented
			"create_heightmap" function is implemented
			"create_indices" function is implemented
			"setup_heightmap" function is implemented

Credit:
	lines 88-95 and 155-162:  https://learnopengl.com/Guest-Articles/2021/Tessellation/Height-map
							  helped with creating indices and using the glDrawElements to draw from array