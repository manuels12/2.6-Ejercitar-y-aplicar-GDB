# 2.6.Ejercitar y aplicar GDB (debugger) en su QEMU-Raspbian virtual 
* * *
Este fue el programa que se uso que se llamo use_gdb.s
~~~
@ use_gdb.s
@ demo program
.section	.data
.section	.text
.globl		_start
_start:
mov r1, $5	@ load r1 with 5
cmp r1, $4	@ compare r1 with 4
sub r1, r1, $1	@ subtract 1 
cmp r1, $4      @ r1 now DOES equal 4
sub r1, r1, $1
cmp r1, $4

mov r7, $1	@ exit syscall
svc $0		@ wake kernel
.end
~~~
Aqui se muestra la crecacion y los comandos pertinentes para correrlo, el codigo en este archvivo que creamos es el anterior (use_gdb.s)
![](2.6.png)
* * *
Al correrlo nos arroja esto 
![](2.66.png)
* * *
Y esto
![](2.666.png)
* * *
![](2.66666.png)
* * *
![](2.6666666.png)
* * *
