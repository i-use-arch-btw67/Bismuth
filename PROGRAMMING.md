# How do you program the chip?

the programming of the chip is relatively simple. to program it you first need to understand what every section of an instruction does.
the first 4 bits select the MUX operation, the next 32 choose how big A and B are, after that the next bit chooses between using the register's value or A, the next bit chooses whether to write to the cache or not, the last bit clears the cache.
to program the chip you need to convert your 43 bit binary into 11 bit hex because that is the only thing the ROM supports.

# INSTRUCTIONS

0000	ADD

0001  SUB

0010  MULT

0011  AND

0100  OR

0101  NOR

0110  XOR

0111  SHIFT A LEFT

1000  SHIFT A RIGHT

# Program example

00005000282

00000000186

08000000306

10000000186


this program calculates 10 + 5, register result + 3, 18 - 6, 12 × 3
