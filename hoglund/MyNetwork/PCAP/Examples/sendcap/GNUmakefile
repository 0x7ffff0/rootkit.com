PCAP_PATH = ../../lib
CFLAGS = -g -O -mno-cygwin -I ../../include -DWPCAP

OBJS = sendcap.o
LIBS = -L ${PCAP_PATH} -lwpcap

all: ${OBJS}
	${CC} ${CFLAGS} -o sendcap.exe ${OBJS} ${LIBS}

clean:
	rm -f ${OBJS} sendcap.exe

.c.o:
	${CC} ${CFLAGS} -c -o $*.o $<
