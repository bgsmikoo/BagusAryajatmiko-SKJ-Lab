# Makefile for assembly to C++ conversion project

# Compiler and flags
CXX = g++
CXXFLAGS = -o

# Target to compile the program
all: M1_T2.exe

# Compiles M1_T2.cpp into an executable
M1_T2.exe: M1_T2.cpp
	$(CXX) $(CXXFLAGS) M1_T2 M1_T2.cpp

# Target to disassemble the compiled code
dump: M1_T2.exe
	objdump -d -j .text M1_T2.exe > M1_T2.asm

# Target to clean up generated files (Windows version)
clean:
	del /f M1_T2.exe M1_T2.asm

# Target to run the compiled executable
run: M1_T2.exe
	./M1_T2.exe
