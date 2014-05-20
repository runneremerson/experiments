all:QueryServer

QueryServer:QueryServer.o
	gcc -o $@ $^  -L/usr/local/lib  -lzookeeper_mt

QueryServer.o:QueryServer.c
	gcc -DTHREADED -I/usr/local/include/zookeeper -o $@ -c $^

.PHONY:clean

clean:
	rm QueryServer.o QueryServer
