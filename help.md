### gdb命令使用手册
gcc option: -ggdb3 -O0

```
start: 开始调试
n    : 执行单条指令(不进入函数)
s    : 单步调试(进入函数)
b    : 设置断点
    b 行号
    b 函数名
    b 文件名:行号
    b 文件名:函数名
    b +num
    b -num
bt    : 查看函数调用栈贞
i locals : 查看所有局部变量
i b  : 查看所有断点
delete <b编号> : 删除某个断点
clear : 删除所有断点
p : 打印变量值
set var num = xxx : 设置变量值
display arr@len: display array for length
util num: run line number
finish : 结束当前函数调试
c : 继续执行到下一个断点
r : 重新开始调试
watch 变量 : 监测变量变化时，暂停
i watchpoints ： 查看所有监测点
i registers : 显示寄存器信息
catch <事件名称>(throw/catch/exec/fork/vfork/load/unload) ：发生相应事件时，暂停
set follow-fork-mode child: bind child process
set detach-on-fork off: bind child process
```
