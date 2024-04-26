CC = gcc
CFLAGS = -Wall
LDFLAGS_SERVER = -pthread
TARGET_SERVER = HTTP_Server
TARGET_CLIENT = HTTP_Client

all: $(TARGET_SERVER) $(TARGET_CLIENT)

$(TARGET_SERVER): HTTP_Server.c
	$(CC) $^ -o $@ $(LDFLAGS_SERVER)

$(TARGET_CLIENT): HTTP_Client.c
	$(CC) $^ -o $@ $(CFLAGS)

%.o: %.c
	$(CC) -c $
clean:
	rm -f *.o $(TARGET_SERVER) $(TARGET_CLIENT)
