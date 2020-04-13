OS := $(shell uname)
OPTIONS:=

ifeq ($(OS),Darwin)
	OPTIONS += -framework OpenCL
else
	OPTIONS += -l OpenCL
endif

main: host.cpp
	g++ -Wall -g host.cpp -o main $(OPTIONS)

clean:
	rm -rf main
