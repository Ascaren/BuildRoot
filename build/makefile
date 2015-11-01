CC=../../i686-buildroot-linux-uclibc-gcc-4.9.3
#CC=gcc

All: clean Lib Exe

Lib:
	$(CC) -fPIC ../src/multiplication.c -shared -o libmultiplication.so

Exe:
	$(CC) ../src/main.c -L. -lmultiplication -o multiplication

clean:
	rm -f libmultiplication.so
	rm -f multiplication
