## 通用寄存器
EAX 累加
```
  ;  32位变量加1 
  mov eax, dword ptr[ebp-4]
  add eax, 1
  mov dword ptr[ebp-4]
```

EBX 基址
```
  mov eax, dword ptr[ebpx+8]
```


ECX 计数
```
  mov ecx, 0Ah
label:
  add eax, ed
  loop label    ; ecx --
```

EDX 数据
```
  mov ebx, 10h
  div ebx       ; EAX / EBX 
```


## 变址寄存器
ESI: 源变址寄存器
EDI: 源变址寄存器


```
  ; copy 32位值
  mov ecx, 10h
  rep movs dword ptr[edi], dword ptr[esi]
```

## 指针寄存器
EBP : 基址指针寄存器
ESP : 堆栈指针寄存器
EIP : 指令指针寄存器

```
  push esp
  mov  ebp, esp
  sub  esp, 0Ch
  push esi
  push edi
  cmp  dword ptr[ebp+8], 0
```

## EFLAGS



