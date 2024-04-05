# all:
# 	g++ HelloWorld_Cplusplus.cpp

# clean: 
# 	rm 
# Compiler
CC = g++

# Compiler flags
CFLAGS = -std=c++11 -Wall

# Source files
SRCS = HelloWorld_Cplusplus.cpp

# Object files
OBJS = $(SRCS:.cpp=.o)

# Executable name
EXEC = myprogram

# Default target
all: $(EXEC)

# Compile source files into object files
%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

# Link object files into the executable
$(EXEC): $(OBJS)
	$(CC) $(OBJS) -o $(EXEC)

# Clean up intermediate object files and the executable
clean:
	rm -f $(OBJS) $(EXEC)