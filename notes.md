
## commands

s: seek  

V: visual mode（可视化模式）    

进入函数: 先seek到函数地址，enter进入，u返回  


### V (Visual Mode)

p: switch views（切换视图）  

;: comments


### a

aaa: analyze all  

afl: analyze function list (function symbols，函数符号)  

afll: verbose mode of afl  

axt: analyze xref to，交叉引用到，要先seek选中函数  


### i

ii: Imports(导入函数)  

iE: Exports(导出函数)  

is: symbols(所有符号)  

iS: Sections(节)  

iz: search Strings in .rodata section  

izz: search Strings in the whole binary  


### w (writing / patching)

在Visual mode下，按A修改opcode  


### d

aaa，afl  

按V，按p切换到debug view   

db: set breakpoint  

dc: continue ('c' in gdb)

do: reopen ('r' in gdb)  

F7: step into  

F8: step over  

F9: run

dsf: step until end of frame ('finish' in gdb)  


### VV (Gragh Mode)

aaa

p: switch views

进入函数: [ga], [gb], [gc]

x: xref



### How to solve a real game

> r2 -d a.out

1. aaa

2. ia

3. iz, izz

4. afl

5. db main

6. s main

7. V, p

8. dc / F9, F7, F8

9. px @ 0xdeadbeef

10. ood