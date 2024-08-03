# Compiler
CC = clang

# Source file and output executable
SRC = src/hello/hello.c
EXEC = target/hello/program

all : clean build run

# Default target
build: $(EXEC)

# Build the executable. @ hides the comand being printed
$(EXEC): $(SRC)
	@$(CC) $(SRC) -o $(EXEC)

# Run the executable
run:
	./$(EXEC)

# Clean up the executable
clean:
	@rm -f $(EXEC)

# Phony target to avoid conflicts with file names
.PHONY: build clean
