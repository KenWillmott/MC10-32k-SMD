MC10-32k-SMD
A 32k memory upgrade PCB for the Radio Shack MC-10 microcomputer. It replaces the two 2kb RAM chips in the MC-10. The minimal install gives you contiguous memory from 0x0000 to 0x7FFF (except for the CPU registers in low memory). So stock Micro Color Basic recognizes and uses the the upper 16k of that, and the lower half is available for general or machine language use. There are two options:
1. Page select inputs: board inputs L0 and L1 can be connected to any digital outputs, then they will select one of four video page addresses as follows:
   <img width="551" height="155" alt="mc10-modes-latch" src="https://github.com/user-attachments/assets/d582ab57-7651-4385-8e22-c5a0297ea55a" />
2. Battery backup: when U4 DS1210 is installed, and 3.0V is provided at the EXT BATT terminals, the memory becomes non-volatile (contents remain while main power is removed)
