
## commands

s : seek  

V : visual mode（可视化模式）  

p : switch views（切换视图）  

进入函数 : 先seek到函数地址，enter进入，u返回  


### a

aaa : analyze all  

afl : analyze function list (function symbols，函数符号)  

afll : verbose mode of afl  

axt : analyze crossref to，交叉引用到，要先seek选中函数  


### i

ii : Imports(导入函数)  

iE : Exports(导出函数)  

is : symbols(所有符号)  

iS : Sections(节)  

iz : search Strings in .rodata section  

izz : search Strings in the whole binary  


### w (writing / patching)

在Visual mode下，按A修改opcode  


### d

第一件事：aaa，afl  

按V，再按p切换到debug视图  

db : set breakpoint  

dc : continue ('c' in gdb)

do : reopen ('r' in gdb)  

F7 : step into  

F8 : step over  

dsf : step until end of frame ('finish' in gdb)  