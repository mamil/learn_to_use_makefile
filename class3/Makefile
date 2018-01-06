#加入一个变量，免得重复写
OBJS = main.o wood.o gold.o

#.o文件的生成方式，也可以自动推导
main : $(OBJS)
	g++ -o main $(OBJS)


#rm -f 可以忽略错误，文件不存在也不会报错
clean: 
	rm -f main $(OBJS)
