CFLAGS=-m32 -g

all: integrate


integrate: integrate.o
	gcc $(CFLAGS) -o $@ $^

%.o: %.asm
	yasm -f elf32 -g dwarf2 -o $@ $^
