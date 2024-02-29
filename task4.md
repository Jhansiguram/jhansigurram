# **The C code should undergo the simulation of normal GCC X86 Compiler and riscv compiler** (**SPIKE Simulation**) 

**AS PER THE REQUIREMENT OUTPUT OF GCC (F1) SHOULD BE EQUAL = TO OUTPUT OF RISCV GCC (F2)**
![j1](https://github.com/Jhansiguram/jhansigurram/assets/160741021/68244cf2-c8b0-40f9-b02f-d8614864432f)
**Step - 1**: To Run the code in the normal GCC Compiler</p>


  To compile the code: 
            
        gcc sum1ton.c -o sum1ton
   To Get the output use:
       
       ./a.out
  Here the output finds to be -Sum of numbers from 1 to 250 is 31375

![j2](https://github.com/Jhansiguram/jhansigurram/assets/160741021/41246489-d07b-4a4c-a256-24c7a052e8f7)
**Step - 2**: To Run the code in the RISC-V GCC Compiler</p>
To compile the code :</p>

    riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
    gcc sum1ton.c -o sum1ton
    ./sum1ton
 Here the output finds to be -Sum of numbers from 1 to 250 is 31375</p>
 
![j3](https://github.com/Jhansiguram/jhansigurram/assets/160741021/50b521c1-4ab3-4097-bbd9-73ec33369d08)
To compile the code:
  
    riscv64-unknown-elf-gcc -o sum1ton sum1ton.c
  or
    
    riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
  or

    riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
 (by referring the image given below) </p>
 To Get the output use:

    ./a.out
 Here the output also finds to be -Sum of numbers from 1 to 250 is 31375
 
![j4](https://github.com/Jhansiguram/jhansigurram/assets/160741021/34fafb9d-636b-4b0a-878e-0953fe36b5f0)
