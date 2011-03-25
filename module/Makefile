CC = gcc
FLAGS = -m32 -shared -Wall -fPIC -I./ -D_LINUX -fvisibility=hidden

OUTFILE = whirlpool.so

SRC = $(wildcard ./*.c ./*.cpp ./SDK/*.cpp)

all: whirlpool

whirlpool:
	$(CC) $(FLAGS) -o $(OUTFILE) $(SRC)
	strip --strip-unneeded $(OUTFILE)

clean:
	rm -f $(OBJ)
