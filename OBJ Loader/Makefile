CC			= g++

TARGET		= OBJLoader

$(TARGET):	Main.o Init.o Obj.o
	$(CC) -o $(TARGET) Main.o Init.o Obj.o `sdl-config --libs` -lGL -lGLU -lm

Main.o:		Main.cpp main.h
	$(CC) -c Main.cpp `sdl-config --cflags`

Obj.o:	    Obj. p Obj.h
	$(CC) -c Obj.cpp `sdl-config --cflags`

Init.o:		Init.cpp main.h
	$(CC) -c Init.cpp `sdl-config --cflags`

clean:
	rm -f $(TARGET) Main.o Init.o Obj.o core
