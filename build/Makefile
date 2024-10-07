flags = -O2 -Wall -std=c2x
ldflags =

all: clean aurora

aurora: src/aurora.o
	cc $(flags) $^ -o $@ $(ldflags)

src/aurora.o: src/aurora.c
	cc $(flags) -c $< -o $@

clean:
	rm -f src/*.o aurora