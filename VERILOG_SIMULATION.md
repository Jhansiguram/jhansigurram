# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I

![Screenshot 2024-03-05 133127](https://github.com/Jhansiguram/jhansigurram/assets/160741021/134dd906-487f-4c07-9463-b699cbaf800c)
## 3. INSTRUCTION SET OF RISC-V RV32I

![Screenshot 2024-03-05 133150](https://github.com/Jhansiguram/jhansigurram/assets/160741021/eee9d7cd-130a-4296-a5d4-a4061616d522)

![Screenshot 2024-03-05 133204](https://github.com/Jhansiguram/jhansigurram/assets/160741021/a9a05925-b786-4e7e-b51c-11f9eebcc1f8)
## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.
  
### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**

 Open your terminal and type the following to install iverilog and GTKWave
 ```
 $   sudo apt get update
 $   sudo apt get install iverilog gtkwave
 ```

![w1](https://github.com/Jhansiguram/jhansigurram/assets/160741021/34bf6810-3d75-4103-b896-b59f2ade49d9)
- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
 $ git clone https://github.com/Jhansigurram/Jhansigurram
 $ cd Jhansigurram
```

![w2](https://github.com/Jhansiguram/jhansigurram/assets/160741021/afb06556-97b7-4658-acd3-07ddb856132a)
- **To simulate and run the Verilog code, enter the following commands in your terminal.**

```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
```

![w3](https://github.com/Jhansiguram/jhansigurram/assets/160741021/ea576be3-957f-4200-a26a-02bc7a6280d5)
- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`

![w4](https://github.com/Jhansiguram/jhansigurram/assets/160741021/73430859-ebb9-41d8-8a7c-1e6dc6edce0e)
### 4.3 The output waveform

 The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
 Instruction 1:add r6,r2,r1
 ![Screenshot 2024-03-05 133253](https://github.com/Jhansiguram/jhansigurram/assets/160741021/ce41892e-2ce7-4be4-8923-5f470eeb8a4b)
 Instruction 2:sub r7,r1,r2
 ![Screenshot 2024-03-05 133309](https://github.com/Jhansiguram/jhansigurram/assets/160741021/6133576e-b922-4441-8f4b-be2484d08861)
 Instruction 3:and r8,r1,r3
 ![Screenshot 2024-03-05 133321](https://github.com/Jhansiguram/jhansigurram/assets/160741021/100b91db-03f0-48f9-86dd-cdb040b05085)
 Instruction 4:or r9,r2,r5
 ![Screenshot 2024-03-05 133339](https://github.com/Jhansiguram/jhansigurram/assets/160741021/945325ae-98ad-4d26-bf1b-d990957e7b82)
 Instruction 5:xor r10,r1,r4
 ![Screenshot 2024-03-05 133429](https://github.com/Jhansiguram/jhansigurram/assets/160741021/e3e240bf-6378-4002-bb93-e33c69ae6295)
 Instruction 6:slt r11,r2,r4
 ![Screenshot 2024-03-05 133445](https://github.com/Jhansiguram/jhansigurram/assets/160741021/08f6a0da-193e-409a-b8de-812a4050d13e)
 Instruction 7:addi r12,r4,5
 ![Screenshot 2024-03-05 133459](https://github.com/Jhansiguram/jhansigurram/assets/160741021/439b0729-44fb-43a7-9a8c-810ae27fdd12)
 Instruction 8:sw r3,r1,2
 ![Screenshot 2024-03-05 133518](https://github.com/Jhansiguram/jhansigurram/assets/160741021/1b52de95-e6f2-428a-afb3-94c8db6f7d14)
 Instruction 9:lw r13,r1,2
 ![Screenshot 2024-03-05 133534](https://github.com/Jhansiguram/jhansigurram/assets/160741021/a41b17d6-4829-4800-8ae9-d1841fdd29ad)
  Instruction 10:beq r0,r0,15
 ![Screenshot 2024-03-05 133549](https://github.com/Jhansiguram/jhansigurram/assets/160741021/1bb9beb0-8514-42e4-9e41-d99d29a2fdef)
 After branching, performing
 Instruction 11:add r14,r2,r2
 ![Screenshot 2024-03-05 133603](https://github.com/Jhansiguram/jhansigurram/assets/160741021/b9bedade-02be-4ade-b79f-87e409ac09da)
 Full 5-stage instruction pipeline and pc-increment description Waveform
 ![Screenshot 2024-03-05 133625](https://github.com/Jhansiguram/jhansigurram/assets/160741021/47b46f89-1cfc-4b11-9eed-3691c29f6bbc) 
 ![l1](https://github.com/Jhansiguram/jhansigurram/assets/160741021/fe36b352-c788-45a7-bcd4-77f370fb977e)
  ![l2](https://github.com/Jhansiguram/jhansigurram/assets/160741021/b20c2a5b-0b9b-47a6-a7ea-b497e4801ead)
