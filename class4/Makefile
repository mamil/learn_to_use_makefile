#指定源文件目录
SRCS += $(wildcard src/*.cpp)

#指定编译选项，这里包含头文件的文件夹
CFLAGS += -Iinclude

#指定目标
TARGET += main

#生成.o文件名字
#这里要提醒一下，函数的命令界线是,
#然后就是类似c++的宏展开，你可以试一下这个，有什么区别，用下面新增的函数debug一下
#OBJS = $(subst .cpp, .o, $(SRCS))
OBJS = $(subst .cpp,.o, $(SRCS))

#.o文件的生成方式，也可以自动推导
$(TARGET) : $(OBJS)
	g++ $(CFLAGS) -o $(TARGET) $(OBJS)


#rm -f 可以忽略错误，文件不存在也不会报错
clean: 
	rm -f $(TARGET) $(OBJS)




####################################
#加一个在Stack Overflow上看到的用法，对调试Makefile很有用
print-%: ;@echo $* = $($*)

#比如定义变量
HAHA = "hahahahaha"
#直接用make print-HAHA 
#就可以看到HAHA的值了
#在这个文件里面，可以print-SRCS
#看看源文件有哪些
