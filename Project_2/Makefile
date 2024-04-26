CC =gcc
CFLAGS =-Wall
LDFLAGS =-pthread
TARGET_SERVER =HTTP_Server.c
TARGET_CLIENT =HTTP_Client.c

all: $(TARGET_SERVER) $(TARGET_CLIENT)

$(TARGET_SERVER): HTTP_Server.o
	$(CC) $(LDFLAGS) $^ -o $@

$(TARGET_CLIENT): HTTP_Client.o
	$(CC) $^ -o $@

%.o: %.c
	$(CC) $(CFLAGS) $< -o $@

clean:
	rm -f *.o $(TARGET_SERVER) $(TARGET_CLIENT)
