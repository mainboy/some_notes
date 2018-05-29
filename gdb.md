

# 我用的比较多的调试命令





## disassemble

展示当前栈的汇编指令



## objdump

### objdump -d [name of executable] > [any file name]

将执行文件反汇编成普通可查看文件



## info

### info breakpoints
- 展示所有断点信息

### info registers
- 展示寄存器的内容  显示格式：reg Hex dec
- 可带具体参数 如 info registers rax

#### 寄存器

![捕获](https://github.com/mainboy/some_notes/blob/master/%E6%8D%95%E8%8E%B7.PNG)


- rbx: 标识上下文的，函数调用时需要先入栈，函数返回时出栈
- rdi: 记录函数传入的第一个参数
- rsi: 记录函数传入的第二个参数
- rax: 记录函数返回值



## print

### print /x [ addr | mem[addr] ]
- Hex格式打印地址或地址上的内容

### print (char*)addr
- 打印地址上的字符串



## breakpoint

### break *address
- 在地址处设置断点

### break function
- 在函数处设置断点
