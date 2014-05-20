all:Election

Election:Election.o
	gcc -o $@ $^  -L/usr/local/lib -lzookeeper_mt 

Election.o:Election.c
	gcc -g -DTHREADED -std=c99 -I/usr/local/include/zookeeper -o $@ -c $^

.PHONY:clean

clean:
	rm Election.o Election
