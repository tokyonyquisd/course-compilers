# course-compilers
berotiny pascal porting win32 -> linux64

compile:

     gcc -c beronew.s
     ld beronew.o -g -o beronewNolib
     gdb beronewNolib 

SASM compiler config:
x64 GAS

     as -o $PROGRAM.OBJ$ $SOURCE$
     ld $PROGRAM.OBJ$ -g -o $PROGRAM$

gas:

    (IsEOF) == IsEOF

gdb:

    info files
    b *0x4000b0
    run == r
    si 3
    ni 3
    x/5i $pc
    x/8g $sp
    info registers == i r
    p $rax
    set $rax = 0x123
