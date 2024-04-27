To perform addition using ARM64 instruction set, we would typically use assembly language. However, since you requested the binary representation, let's break down the process into binary representation steps.

ARM64 instructions typically involve register operations. We'll represent the addition of 1 and 2 using ARM64 assembly instructions and then convert them into binary.

Here's the ARM64 assembly code for adding 1 and 2:

```
mov w0, #1      // Move the value 1 into register w0
mov w1, #2      // Move the value 2 into register w1
add w2, w0, w1  // Add the values in registers w0 and w1, store the result in register w2
```
Now, let's convert these instructions into binary representation:

mov w0, #1
OpCode: mov (Move operation)
Register: w0 (Destination register)
Immediate/Data: #1 (Immediate value to move)
```
OpCode:            1001
Register (w0):     00000
Immediate/Data:    00000000000000000000000000000001 (1 in binary)
```
mov w1, #2
OpCode: mov
Register: w1
Immediate/Data: #2
```
OpCode:            1001
Register (w1):     00001
Immediate/Data:    00000000000000000000000000000010 (2 in binary)
```
add w2, w0, w1
OpCode: add (Addition operation)
Destination Register: w2
Source Register 1: w0
Source Register 2: w1
Binary Representation:
```
OpCode:            10001011000
Register (Destination): 00010 (w2)
Register (Source 1): 00000 (w0)
Register (Source 2): 00001 (w1)
```
Now, if we concatenate these binary representations, we get the binary representation of the complete instruction sequence.

Please note that the actual encoding may vary depending on the specifics of the ARM64 architecture and the assembler being used. So do not be suprised if i am wrong.
