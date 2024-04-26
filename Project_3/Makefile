CC = gcc
CFLAGS = -Wall
TARGET = NTP_and_Localtime_Client

all: $(TARGET)

$(TARGET): NTP_and_Localtime_Client.c
	$(CC) $^ -o $@

%.o: %.c
	$(CC) -c $(CFLAGS) $

clean:
	rm -f *.o $(TARGET)
