# compiler
CC = gcc
CFLAGS += -Wall -Wextra -pedantic-errors

# the sfml libs
LDLIBS := -lm -I.

BIN_DIR = ./bin
SOURCES = test.c

# list of bins
LIST = $(BIN_DIR)/PerlinNoise

all: $(LIST)

# what to do?
$(BIN_DIR)/%: $(SOURCES)
	$(CC) $(CFLAGS) $< $(LDLIBS) -o $@

# remove the binary
clean:
	$(RM) $(BIN_DIR)/*