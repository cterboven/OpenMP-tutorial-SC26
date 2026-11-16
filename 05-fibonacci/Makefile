BIN_DIR=bin
PROGRAM=$(BIN_DIR)/fibonacci

CC=gcc
CFLAGS=-std=c99 -g -O2 -fopenmp
# DEBUG=-DDUMP_TREE=1

all: $(PROGRAM)

$(PROGRAM): fibonacci.c
	$(CC) $(CFLAGS) $(DEBUG) -o $@ $<

$(BIN_DIR): 
	mkdir $@

clean:
	rm -f $(PROGRAM)

wipe: clean
	rm -f *.o *.bak *~
