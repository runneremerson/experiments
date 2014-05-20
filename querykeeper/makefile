all:QueryServerd

QueryServerd:QueryServerd.o
	gcc -o $@ $^  -L/usr/local/lib -lzookeeper_mt 

QueryServerd.o:QueryServerd.c
	gcc -g -DTHREADED -I/usr/local/include/zookeeper -o $@ -c $^

.PHONY:clean

clean:
	rm QueryServerd.o QueryServerd
