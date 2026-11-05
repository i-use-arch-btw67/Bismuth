# Bismuth
Bismuth is a 16-bit CPU that uses my own yet unnamed ISA.

# How do you program it?

To program the chip you need to know what each bit in the ROM is doing.
the first 4 bits are for selecting the operation that the ALU will perform:

0000 = ADD
0001 = SUB
0010 = MULT
0011 = AND
0100 = OR
0101 = NOR
0110 = XOR
0111 = SHIFT A LEFT
1000 = SHIFT A RIGHT

note: the ALU instructions aren't finished yet so expect more of them!

after the initial 4 bits we have the numbers you want to put together like A and B.
after that we have 4 more bits designated for the amount of shifting A, only useful if the SHIFT command is used.

the last 3 bits are for:

selecting between using A or the register output
