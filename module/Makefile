CC = g++
FLAGS = -m32 -shared -Wall -fPIC -I./

OUTFILE = whirlpool.so

SRC = $(wildcard ./*.cpp ./SDK/*.cpp)

all: whirlpool

whirlpool:
	$(CC) $(FLAGS) -o $(OUTFILE) $(SRC)
	strip --strip-unneeded $(OUTFILE)

clean:
	rm -f $(OBJ)
