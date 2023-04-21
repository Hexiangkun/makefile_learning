#定义依赖变量
src = sub.o add.o div.o multi.o main.o

#定义目标变量
target = app

$(target) : $(src)
	$(CC) $(src) -o $(target)

%.o : %.c
	$(CC) -c $< -o $@

# app : add.o sub.o div.o multi.o main.o
# 	gcc add.o sub.o div.o multi.o main.o -o app

# sub.o : sub.c
# 	gcc -c sub.c -o sub.o

# add.o : add.c
# 	gcc -c add.c -o add.o

# div.o : div.c
# 	gcc -c div.c -o div.o

# multi.o : multi.c
# 	gcc -c multi.c -o multi.o

# main.o : main.c
# 	gcc -c main.c -o main.o