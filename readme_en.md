# CryptoAsm
CryptoAsm is a virtual assembler.
You can execute only one instruction, move data.
It helps to understand pointers in C language.

## register
Registers are a and p.
p points to memory address.

    mov p, a

This puts the value of the register a in the register p.

## number
    mov a, 1

 This puts 1 in the register a.

## memory
There are address 0 to 6 in memory whitch store the data.

## variable
You can use the variables i, j, k and the array l.
Variable i stores the value at memory 0, j at address 1, and k at address 2.

    mov j, a

This stores the value of register a in variable j, that is, address 1 of memory.

    mov a, k

This puts variable k, that is, the value of address 1 of memory in register a.

## array
The array are l [0], l [1], l [2].
Their address is 3, 4 and 5, respectively.

    mov a, l [1]

This puts the value of array l[1], that is, memory 4 address, into the register a.

    mov l [0], a

This puts the value of a register in array l [0], that is, memory 3 address.

## Pointer
The register p holds the address and reads and  writes the data at the address.
You can access the address indicated by the register p.

    mov p,1
    mov a,*p

This puts 1 in the register p.
And  this puts the contents of address 1 to the register a.

When the contents of address 1 is 10, it is 10,
When the contents of address 1 is 20, 20 is put in the register a.

    mov p,2
    mov *p,a

This puts 2 in the register p.
And this puts the contents of register a to address 2.

## Pointer 2

    mov p,2
    mov *p+1,a

This puts 2 in the register p.
and this puts the value of the register a at address 3.

## Address

    mov p,&j

It puts the address of the variable j in the register p.
Because variable j's address is 1, it puts the number 1 in p.

There are no instructions below.

    mov &j,p  ;(NG)

&j means number 1. The value of the p register can not be set to 1 in the numeric value.

## Instruction lines
Instructions to be executed are listed.
You can edit it line by line.

## step execution button
Press step to execute one instruction at a time.

## reset execution button
Press reset to return to the first instruction.

## insert button
You can increase the number of instruction lines by pressing insert.
