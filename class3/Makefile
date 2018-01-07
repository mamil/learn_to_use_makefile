#加入一个变量，免得重复写
OBJS = main.o wood.o gold.o

#.o文件的生成方式，也可以自动推导
main : $(OBJS)
	g++ -o main $(OBJS)


#rm -f 可以忽略错误，文件不存在也不会报错
clean: 
	rm -f main $(OBJS)


####################################
#加一个在Stack Overflow上看到的用法，对调试Makefile很有用
print-%: ;@echo $* = $($*)

#比如定义变量
HAHA = "hahahahaha"
#直接用make print-HAHA 
#就可以看到HAHA的值了
#在这个文件里面，可以print-OBJS
#看看源文件有哪些