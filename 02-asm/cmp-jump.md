
## test , cmp

test属于逻辑运算指令, 执行BIT与BIT之间的逻辑运算

Test的一个非常普遍的用法是用来测试一方寄存器是否为空:

test ecx, ecx
jz somewhere

如果ecx为零,设置ZF零标志为1,Jz跳转



CMP属于算术运算指令, 比较两个值(寄存器,内存,直接数值)
语法: CMP r/m,r/m/data
标志位: C,P,A,Z,O

CMP比较.(两操作数作减法,仅修改标志位,不回送结果).
cmp实际上是只设置标志不保存结构的减法,并设置Z-flag(零标志).
零标志很像carry,也是内部标志寄存器的一位.


## jmp
jpm (EB)  
je  (74)
jz  (84)


