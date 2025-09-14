#指定编译器
CC = gcc

#编译选项
CFLAGS = -g -O2 -Wall -Werror -I include


# TODO

all: hello
	echo "Build complete!"
clean:
	rm -f *.o

hello: hello.o add.o mu.o
	$(CC) $(CFLAGS) hello.o add.o mu.o -o hello

hello.o: hello.c
	$(CC) $(CFLAGS) -c hello.c -o hello.o

add.o: add.c
	$(CC) $(CFLAGS) -c add.c -o add.o

mu.o: mu.c
	$(CC) $(CFLAGS) -c mu.c -o mu.o
.PHONY: all clean
