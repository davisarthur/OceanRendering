grayscale_OBJECTS:= grayscale.out
render_OBJECTS:= render.out
sky_OBJECTS:= sky.out
tiling_OBJECTS:= tiling.out

default: grayscale render sky tiling

grayscale:
	g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp grayscale.cpp -o grayscale.out
render:
	g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp render.cpp -o render.out
sky:
	g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp sky.cpp -o sky.out
tiling:
	g++ -lglfw -lglew -framework OpenGL helperFunctions.cpp tiling.cpp -o tiling.out