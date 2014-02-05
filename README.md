MIPS CPU Simulator
==================

This is a MIPS processor prototype written in C language.

It Simulates MIPS processor running states: instruction fetch, decode, execute, pc update, exception handler.

It also provides basic debug functions for MIPS ASM programs: next, step, breakpoint, run, memory/register watch and PC jump.

My project: https://github.com/hdl/mips is written in VHDL based on this prototype.

==================
###gccmips_elf and other tools: 
The binary tools for analysis of ELF file. 

###kernel:
Real Time Operating System which can run on project: https://github.com/hdl/mips

###tools:
Check Makefile to compile

make mlite: MIPS CPU Simulator

make bootldr: Boot Loader for elf file and kernel

make hello: hello world...

boot.asm: Interrupt Service Routine inside.

###mlite:
make mlite

Provided basic debug functions for MIPS ASM programs: next, step, breakpoint, run, memory/register watch, pc jump.

Simulated MIPS processor running states: instruction fetch, decode, execute, pc update, exception handler.

###boot loadder:
make bootldr

Assembly code initializes stack pointer, sets interrupt service routine and jumps to main().

Initializes hardware, prepares RAM space for kernel or ELF programs.

Provides basic boot loader functions: memory read, write, dump and binary file receiving (serial port).


###More information please check http://opencores.org/project,plasma

