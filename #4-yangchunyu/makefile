CC = gcc
CFLAGS = -g -O2 -Wall -Werror -I$(INCLUDE_DIR)
TARGET = program

SRC_DIR = lib
INCLUDE_DIR = include

SRCS = $(SRC_DIR)/add.c $(SRC_DIR)/mu.c

OBJS = $(SRCS:.c=.o)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

$(SRC_DIR)/%.o: $(SRC_DIR)/%.c
	$(CC) $(CFLAGS) -c $< -o $@


clean:
	rm -f $(OBJS) $(TARGET) *.out

.PHONY: clean
