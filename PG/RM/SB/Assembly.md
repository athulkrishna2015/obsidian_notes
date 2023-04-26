- directive (pseudo-instruction) is only for the assembler. Eg. ORG, END tells the assembler where to put the opcode or where the program (source code) ends
- An assembly language instruction consists of four fields:
 [label:] mnemonic [operands] ;[comment]
  - Labels are used to refer to a line of the code by name. They are followed by a colon “:"
 - These lines could instead be directives or pseudo-instructions. They do not generate any opcodes (machine codes) 
- The PC in 8051 is 16 bits wide, so it can access program addresses from 0000H to FFFFH, a total of 64K of byte codes
- A register is required to indicate arithmetic conditions like the carry bit.
- This register in 8051 is called Program Status Word or (PSW) register. 
  - It has 8 bits but only 6 are used by 8051 rest two are for user-definable
  
| CY  | PSW.7 | Carry flag.                                                |
| --- | ----- | ---------------------------------------------------------- |
| AC  | PSW.6 | Auxiliary carry flag.                                      |
| F0  | PSW.5 | Available to the user for general purpose.                 |
| RS1 | PSW.4 | Register Bank selector bit 1.                              |
| RS0 | PSW.3 | Register Bank selector bit 0.                              |
| OV  | PSW.2 | Overflow flag.                                             |
| --  | PSW.1 | User-definable bit.                                        |
| P   | PSW.O | Parity flag. Set/cleared by hardware each instuction cycle |
```
MOV A,#88H
ADD A,#93H ;after the addition 
            A=1BH,CY=1   
```
#### RAM In 8051
- 8051 has total 128 bytes of RAM which are from addresses 00H to 7FH.
- The RAM is divided into three regions: 
  1. Register Banks and Stack, 
    - Locations 00H to 1FH (32== 8x4 locations) are set aside for register banks 0, 1, 2 and 3. 
    - Each ===bank has 8 memory locations called R0 to R7. 
    - Thus the register bank 1 R0-R7 are from 00H to 07H, bank 2 from 08H to 0FH, bank 3 from 10H to 17H and bank 4 from 18H to 1FH.
    - To switch from bank 0 to any other bank, the bits 3 and 4 of PSW are changed accordingly 
|  | RS1(PSW.4) | Rs0(PSW.3) |
| --- | --- | --- |
| Bank 0 |0 |0
|Bank 1 |0 |1
|Bank 2| 1 |0
| Bank 3| 1 |1 |
#### Stack and Stack Pointer
- Stack is a region in RAM used by CPU store information temporarily.	
- It is by default in the same location as bank 1, i.e. from locations 07H to 0FH.
- The Stack Pointer is a register which keeps track of where the Stack is. The SP is 8 bits wide, so the stack can be at  addresses between 00H to FFH. By 
- default when 8051 powers up the SP is 07H. Thus the first location used by the

stack in 8051 is 08H. • The storing of a regist
  1. bit addressable memory 
  2.  scratch pad.
- 
