CC			= g++ -ggdb

TARGET		= MultiTexturing

$(TARGET):	Main.o Init.o
	$(CC) -o $(TARGET) Main.o Init.o `sdl-config --libs` -lGL -lGLU -lm

Main.o:		Main.cpp main.h
	$(CC) -c Main.cpp `sdl-config --cflags`

Init.o:		Init.cp main.h
	$(CC) -c Init.cpp `sdl-config --cflags`

clean:
	rm -f $(TARGET) Main.o Init.o core
