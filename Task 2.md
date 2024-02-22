# Let's learn various types of RISC-V instructions
<p align="justify">RISC-V instructions are encoded using a fixed-length 32-bit format, which simplifies decoding and execution. The instruction formats are categorized into six types: R, I, S, B, U, and J. Each format serves a specific purpose and has a unique encoding structure:</p>

<details>
<summary><b>R-type instructions:
</b></summary>
<br>
<p align="justify">In RISC-V, R-type instructions are a type of instruction format used for arithmetic and logical operations that operate on registers. Eg:- add x1, x2, x3
</p>
  </details>
<details>
<summary><b>I-type instructions:
</b></summary>
<br>
<p align="justify">These instructions are commonly used for operations that involve loading immediate values into registers, arithmetic/logical operations with an immediate operand, or branching with immediate offsets.Eg:-opcode rd, rs1, imm

</p>
  </details>
<details>
<summary><b>S-type instructions:
</b></summary>
<br>
<p align="justify"> These instructions typically take one register as a source (for the value to be stored) and an immediate offset to calculate the memory address where the value will be stored. Eg:- opcode rs2, imm(rs1)

</p>
  </details>
<details>
<summary><b>B-type instructions:
</b></summary>
<br>
<p align="justify">These instructions allow the program to alter the flow of control based on the result of a comparison between two values.Eg:- bne x1, x2, 100

</p>
  </details>
<details>
<summary><b>U-type instructions:
</b></summary>
<br>
<p align="justify">These instructions typically involve setting immediate values for certain operations or specifying jump targets.Eg:-lui x1, 0x1000</p>
  </details>
<details>
<summary><b>J-type instructions:
</b></summary>
<br>
<p align="justify">J-type instructions are often used for implementing function calls, loops, and other control flow constructs in programs. Eg:- j 0x80001000
</p>
</details>

# Base Instructions Format

<p align="justify">The basic instruction format in RISC-V is the RISC-V base integer instruction format, which is categorized into different instruction types based on the functionality they provide. 
<details>
<summary><b>Instruction code format </b></summary>
	<br>
![instruction code formats] ![Screenshot 2024-02-22 162716](https://github.com/Jhansiguram/jhansigurram/assets/160741021/de979b34-7d8c-4be0-9554-7696ee6a45b5)

</details>

# RISC-V REGISTER FILE: 

 <p align="justify">The RISC-V register file is a key component of the RISC-V architecture, providing a set of storage locations for holding data during the execution of instructions. The register file is organized into a set of integer registers and floating-point registers, depending on the extensions implemented in the processor. Registers play a crucial role in the RISC-V architecture, as they enable fast access to data and help improve the performance and efficiency of the processor.</p>
