makefile 基本介绍

基本例子

```
username = dalong
main: main.c 
    gcc main.c -o main
.PHONY: clean
clean: 
    echo $(username)
    rm  -rf main
```

说明：

username  ： 我们定义的一个变量

main： target  也就是我们使用make 命令之后开始运行的入口（实际上make 把第一个当作入口和我们命名没关系），其中我们有一个依赖 main.c  具体的操作是使用gcc 进行代码编译

.PHONY:  安全的clean 操作，放置重命名覆盖

clean：  一般做为资源的清理操作，实现make clean 显式执行



备注：

一般makefile 的格式

```
target: dependency
    # 注意是一个tab 距离
    command 
```







