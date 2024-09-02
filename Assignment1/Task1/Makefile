# Makefile for add_numbers project

# Compiler and flags
CXX = g++
CXXFLAGS = -o

# Target to compile the program
all: add_numbers.exe

# Compiles add_numbers.cpp into an executable
add_numbers.exe: add_numbers.cpp
	$(CXX) $(CXXFLAGS) add_numbers add_numbers.cpp

# Target to disassemble the compiled code
dump: add_numbers.exe
	objdump -d -j .text add_numbers.exe > add_numbers.asm

# Target to clean up generated files
clean:
	del /f add_numbers.exe add_numbers.asm

# Target to run the compiled executable
run: add_numbers.exe
	./add_numbers.exe