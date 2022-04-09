CC=gcc
FLAGS=-g -O2 #-Werror -Wextra -Wall -fsanitize=address
TARGET=decimal

all: $(TARGET)

$(TARGET): $(TARGET).o
	$(CC) $(FLAGS) $< -o $@

$(TARGET).o: $(TARGET).c
	$(CC) $(FLAGS) -c $^ -o $@

clean:
	rm -f decimal.o decimal
