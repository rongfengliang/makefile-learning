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



