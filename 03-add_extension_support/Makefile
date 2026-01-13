CC = gcc

CFLAGS= -std=c17 -g -O2
LDFLAGS= -lglfw -lvulkan -ldl -lpthread
SRC= main.c
TARGET= game

$(TARGET): $(SRC)
	$(CC) $(CFLAGS) -o $(TARGET) $(SRC) $(LDFLAGS)

#game:
#	$(CC) $(CFLAGS) -o $(TARGET) $(SRC) $(LDFLAGS)

.PHONY: test clean

test: $(TARGET)
	./ $(TARGET)

clean:
	rm -f $(TARGET)
