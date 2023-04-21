
target = app

src = $(wildcard ./*.c)	#获取当前目录下所有.c文件

objs = $(patsubst %.c, %.o, $(src))	#将src中的每一个元素进行检查，是否符合%.c，符合就替换成%.o

$(target) : $(objs)
	$(CC) $(objs) -o $(target)

%.o : %.c
	$(CC) -c $< -o $@

.PHONY:clean
clean:
	rm -f $(objs) $(target)