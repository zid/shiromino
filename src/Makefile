CFLAGS=-W -Wall -Og -lmingw32 -lSDL2main -lSDL2 -lSDL2_image -lSDL2_mixer -lm
#above should include -m32 if forcing 32 bit

SRC = $(wildcard *.c)
OBJ = $(SRC:.c=.o)

all: game

game: $(OBJ)
	gcc $(OBJ) $(CFLAGS) -o ../game.exe

%.o: %.c
	gcc $^ -c -o $@ $(CFLAGS)

clean:
	rm -f *.o
