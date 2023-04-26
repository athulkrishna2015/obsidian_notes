# binary
## substraction
add one's complimet

# ASCII
- The ACSII system uses a total of 7 bits to represent each code. Example 100 0001($41_d$) is assigned to the upper-case letter "A" and 110 0001 ($61_d$) is for the lower-case letter "a". A zero is placed in the most significant bit position to make it an 8-bit code
- 0-9 are represented by codes 30-39.
- The only bit that is different between the uppercase "A" and lowercase "a" is bit 5. Therefore, conversion between uppercase and lowercase is as simple as changing bit 5 of the ASCII code.

##  Internal Organization of Computers

![[Pasted image 20220516191523.jpg]]

- the CPU is connected to memory and I/O through strips of wire called a bus.
- In every computer, there are three types of buses:
	1.  Address Bus
	2.  Data Bus
	3.  Control Bus /Command Bus
- more address buses available, the larger the number of devices that can be addressed.
- A CPU with 16 address lines can provide a total of 65,536 ($2^{16}$) or 64K of addressable memory.
- Each location can have a maximum if 1 byte of data. This is because all general-purpose microprocessor CPU's are what is called byte addressable.
- To summarize, the total number of memory locations addressable by a given CPU is always equal to $2^x$, where x is the number of address bits, regardless of the size of the data bus.
## Inside Central Processing Units
- Every CPU has what is called a program counter. The function of the program counter is to point to the address of the next instruction to be executed. As each instruction is executed,
- The CPU's program counter can have a value between 0000H and FFFFH.

# Microprosessor Vs Microcontroller
## Micro Prosessor
### 8051
- Majority of 8051 are 8 bit registers.
- Registers are used to store information temporarily.
- ![[Screenshot_20220524_125019.png]]
#### MOV
- MOV destination,source ;copy source to des
- MOV instruction does not affect the source operand.
- to indicate that it is an immediate value it must be preceded with a pound sign (#).
-  “MOV R5 ,#OF9H” that a 0 is used between the # and F to indicate that F is a hex number and not a letters In other words “MOV R5 ,#F9H” will cause an error.
- If values 0 to F are moved into an 8-bit register, the rest of the bits are assumed to be all zeros. For example, in “MOV A, #5” the result will be A = 05; that is, A = 00000101 in binary.
- Moving a value that is too large into a register will cause an error.
	- `MOV A,#7F2H ;ILLEGAL: 7F2H > 8 bits (FFH)`
#### ADD
```
ADD A,source ;ADD the source operand
							;to the accumulator
```
```
MOV A,#25H ;load one operand into A (A=25H)
ADD A,#34H ;add the second operand 34H to A
```
- ADD instruction must always involve register A (Accumulator) and as the destination.


[[SB/Micro controller]]