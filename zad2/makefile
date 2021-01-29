CC=g++

myProgram: main.o employee.o address.o
	$(CC) -o $@ $+

main.o: employee.h address.h
employee.o: address.h

.cpp.o:
	$(CC) -c $<
