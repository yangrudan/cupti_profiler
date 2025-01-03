all: demo

demo: demo.cu
	nvcc -std=c++14 -g -Xcompiler -DNDEBUG -I ../include -I /usr/local/cuda/extras/CUPTI/include -lcuda -L/usr/local/cuda/extras/CUPTI/lib64 -lcupti demo.cu -o demo

clean:
	rm -f *.o demo
