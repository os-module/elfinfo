# elfinfo
将`nm -n`的输出转换为汇编文件，将符号信息写入文件中，具体的格式如下：

```assembly
.section .rodata
.align 3
.global symbol_num
.global symbol_address
.global symbol_index
.global symbol_name
symbol_num:
.quad 0
symbol_address:
symbol_index:
symbol_name:

```

`symbol_num`表示符号数目

`symbol_address`表示符号起始地址

`symbol_index`表示符号的名称起始位置

`symbol_name`部分是符号的名称
