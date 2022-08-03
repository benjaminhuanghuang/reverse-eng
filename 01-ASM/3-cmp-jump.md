
## test , cmp

TEST 做逻辑与(and), 不改变操作数, 只影响标志位ZF

```
; 测试寄存器是否为空, 如果ecx为零,设置ZF零标志为1,JZ跳转  

test ecx, ecx
jz somewhere 
```

CMP: 两操作数作减法,仅修改标志位ZF,不回送结果
语法: CMP r/m,r/m/data
标志位: C,P,A,Z,O
零标志很像carry,也是内部标志寄存器的一位.
```
  ; jump if eax -1 == 0  
  CMP eax, 1
  jz somewhere 
```

## jmp
jpm (EB)  
je  (74)
jz  (84)


