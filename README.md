# 32K-SCMP-in-a-pic
A SC/MP emulator based on the design of the late K. Orton
This is a complete SC/MP computer with 32K RAM and NIBLE write protected in PAGE 0. It has a three 8 bits I/O ports in an 82C55. On port an 8 bits ledbar is connected.
This system can run native SC/MP programs. NIBL uses a soft-UART on 2400 Baud at 20MHz PIC clock frequency (Emulating an ins8060 at 4 MHz)
Flag0 is used as serial out and SB as serial in. In the original SC/MP design Flag0 had to be inverted, but this is done in software in the PIC.
I implemented the HALT instruction that emulates the Elektor halt-reset as can be seen in the schematic. The latest changes by Philg are included.
![scempy2](https://github.com/user-attachments/assets/d5f35d5f-eaa2-4d5f-a04c-a9038ff9e376)
