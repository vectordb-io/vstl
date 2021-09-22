CC:=g++
CFLAGS+=-c -Wall -g -std=c++17
INCLUDES=-I./

OBJS=arrayQueue.o
LIBS=-lpthread 
LFLAGS=-L/usr/local/lib

main: $(OBJS)
	$(CC) $^ -o $@ $(LIBS) $(LFLAGS)

%.o: %.cpp %.h
	$(CC) $(INCLUDES) $(CFLAGS) -o $@ $<

clean:
	rm -rf *.o
	rm -rf main

