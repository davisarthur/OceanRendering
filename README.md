# Ocean Rendering

In this project, I used OpenGL to render simulated ocean waves. To create the simulation, I followed the
approach outlined by Jerry Tessendorf in 
[_Simulating Ocean Water_](https://people.computing.clemson.edu/~jtessen/reports/papers_files/coursenotes2004.pdf).
The project includes 4 demos which can be compiled automatically using the included make file.
If you prefer, I listed manual compilation instructions below.

## Tiling
The ```tiling.cpp``` program renders a large ocean scene by tiling water mesh data stored in a FBO.
This program also supports keyboard and mouse controls to allow the user to move around the scene.
Use the following command to compile this program on Mac:
```
g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp tiling.cpp -o tiling.out
```
On Windows or Linux:
```
g++ -lglfw -lglew helperFunctions.cpp tiling.cpp -o tiling.out
```
Finally, to run the program use the following command: ```./tiling.out```

## Sky
The ```sky.cpp``` program renders a square water mesh and a surrounding skybox. The water is shaded 
using the skybox as an environment map. Use the following command to compile this program on Mac:
```
g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp sky.cpp -o sky.out
```
On Windows or Linux:
```
g++ -lglfw -lglew helperFunctions.cpp sky.cpp -o sky.out
```
Finally, to run the program use the following command: ```./sky.out```

## Render
The ```render.cpp``` program renders and animates a water mesh in 3D using the Fresnel equations to perform shading
Use the following command to compile this program on Mac:
```
g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp render.cpp -o render.out
```
On Windows or Linux:
```
g++ -lglfw -lglew helperFunctions.cpp render.cpp -o render.out
```
Finally, to run the program use the following command: ```./render.out```

## Grayscale
The ```grayscale.cpp``` program renders and animates a wave height map as a 2D grayscale texture.
Use the following command to compile this program on Mac:
```
g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp grayscale.cpp -o grayscale.out
```
On Windows or Linux:
```
g++ -lglfw -lglew helperFunctions.cpp grayscale.cpp -o grayscale.out
```
Once compiled, the program can be run using the following command: ```./grayscale.out```
