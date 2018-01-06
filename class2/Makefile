main : main.o wood.o gold.o
	g++ -o main main.o wood.o gold.o

#下面这些编译条件，以及对应的cpp文件会自动推导，不用自己写了
main.o : wood.h gold.h
wood.o : wood.h headers.h
gold.o : gold.h headers.h

#rm -f 可以忽略错误，文件不存在也不会报错
clean: 
	rm -f main main.o wood.o gold.o
