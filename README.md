# SANEE_RISCV

## Introduction

> The MYTH workshop is an intensive program that guides you through the process of designing a RISC-V based CPU core. In just five days, you'll gain a deep understanding of the RISC-V Instruction Set Architecture (ISA) and implement a simplified RISC-V core with a fundamental instruction set. This repository holds the key to your success in the MYTH workshop.


## **CourseWork**
<details>
<summary>Day 3 : Digital Logic with TL-Verilog in Makerchip IDE</summary>
<br>

Head over to the [MakerChip IDE](https://www.makerchip.com/)
<br>

### A) Inverter

![1](https://github.com/saneeaman9/sanee_riscv/assets/75088597/7984fed0-0c5e-4a5d-a3dc-682cd89a276d)


![2](https://github.com/saneeaman9/sanee_riscv/assets/75088597/c6fb9025-3f66-4658-97f2-c933ec2750d0)


### XOR Gate using Boolean Operator.

![3](https://github.com/saneeaman9/sanee_riscv/assets/75088597/925c331b-2d09-4b42-a52a-76e819a6a9a8)


### C) Vectors

![4](https://github.com/saneeaman9/sanee_riscv/assets/75088597/7699352f-a192-4245-8b99-ce22b6fdbd9f)


### D) Mux

![5](https://github.com/saneeaman9/sanee_riscv/assets/75088597/1095a452-0d39-48fa-a999-354503c91e71)


### E) Simple Calculator
![6](https://github.com/saneeaman9/sanee_riscv/assets/75088597/5ac55944-ccde-4d6d-ba1d-8582ce407e9f)


### F) Fibonacci Series

![7](https://github.com/saneeaman9/sanee_riscv/assets/75088597/66bc4b74-a631-4cc7-a163-f4d100c9469c)


### G) Up Counter

![8](https://github.com/saneeaman9/sanee_riscv/assets/75088597/8adad9e4-7654-43fd-8a7b-b22561d6fc62)


### I) Sequential Calc

![9](https://github.com/saneeaman9/sanee_riscv/assets/75088597/b21d7273-2812-46ff-b443-ffff8bdc6dd1)


### I) Pipelined Logic

#### A simple pipeline through Pythagorean Example.
* Go to "Examples".
* Load Default Template.
* Go to editor and enter the following under TLV.

```bash

`include "sqrt32.v"
|calc
      @1
         $aa_sq[31:0] = $aa[3:0] * $aa;
         $bb_sq[31:0] = $bb[3:0] * $bb;
      @2
         $cc_sq[31:0] = $aa_sq + $bb_sq;
      @3
         $cc[31:0] = sqrt($cc_sq);

```

![10](https://github.com/saneeaman9/sanee_riscv/assets/75088597/45e59958-5d3d-43c0-92ed-a493c634b43a)


### J) Pipeline Implementation example.

![11](https://github.com/saneeaman9/sanee_riscv/assets/75088597/aed76443-b791-4e7a-b163-83a6220d99dd)


### Validity

> - Easier debugging. 
> - Cleaner design.
> - Better error checking.
> - Automated clock gating.


### K) 2 Cycle Calc with Validity.

![12](https://github.com/saneeaman9/sanee_riscv/assets/75088597/402c789a-e5e7-444c-98ce-7358d54ce6c7)


### L) Distance Calc.

![13](https://github.com/saneeaman9/sanee_riscv/assets/75088597/b7dfc9cd-f88a-4b77-8085-214a9ca0acb0)


### Calculator Memory

![14](https://github.com/saneeaman9/sanee_riscv/assets/75088597/8d01f876-87b9-42da-b24d-0b799a10c5a5)




</details>


<details>
<summary>Day 4 : Basic RISC-V CPU Micro Architecture</summary>
</br>

## Overview
This RISC-V Architecture Block Diagram illustrates the fundamental components and their interactions within a computer system based on the RISC-V instruction set architecture. RISC-V is a modular and customizable architecture, providing a versatile framework for designing processors tailored to specific application requirements.

## Components
1. **CPU (Central Processing Unit)**
   - *Description*: The CPU serves as the core of the RISC-V processor, responsible for executing instructions. It includes multiple stages:
     - Instruction Fetch (IF): Fetches instructions from memory.
     - Instruction Decode (ID): Decodes the fetched instructions.
     - Execution (EX): Performs arithmetic and logic operations.
     - Memory (MEM): Manages data memory access.
     - Write Back (WB): Writes results back to registers.

2. **Instruction Memory**
   - *Description*: This memory component stores the program's instructions that the CPU fetches and executes. It's essential for the program's proper execution.

3. **Data Memory**
   - *Description*: Data Memory stores data used by the CPU during program execution. It is crucial for data manipulation and storage.

4. **Registers**
   - *Description*: Registers are a set of general-purpose storage units used for temporary data storage and manipulation by the CPU. They play a pivotal role in instruction execution.

5. **Control Unit**
   - *Description*: The Control Unit manages control signals and coordinates the activities of the CPU's components, ensuring the proper execution of instructions.

6. **ALU (Arithmetic Logic Unit)**
   - *Description*: The ALU performs arithmetic and logic operations as directed by the CPU's instructions. It is the computational workhorse of the processor.

7. **Instruction Decoder**
   - *Description*: The Instruction Decoder interprets and decodes instructions fetched from memory. It translates instructions into actions for the CPU to execute.

8. **Cache Memory**
   - *Description*: Cache Memory provides fast access to frequently used instructions and data. It helps improve the system's overall performance by reducing memory access times.

9. **Bus Interface**
   - *Description*: The Bus Interface facilitates data transfer between the CPU, memory, and peripherals. It ensures efficient communication within the system.

10. **Peripherals**
    - *Description*: Peripherals are external devices such as input/output controllers, timers, and more. They connect to the CPU, enhancing the system's functionality by allowing interaction with the outside world.

For the consecutive labs, we will use the "RISC-V lab starting point code" from https://github.com/stevehoover/RISC-V_MYTH_Workshop.

Use the following [links](DAY 4/day 4 links.txt)

#### 1. Program Counter
![1](https://github.com/saneeaman9/sanee_riscv/assets/75088597/fcb9f75d-d2bb-4ac6-a703-36cab14637e3)

#### 2. Instruction Fetch
![2](https://github.com/saneeaman9/sanee_riscv/assets/75088597/4b7d14a1-7d5c-4b69-b869-dfaf84bb632d)

#### 3. Instruction Decode
![3](https://github.com/saneeaman9/sanee_riscv/assets/75088597/e2a14d26-06df-4ff8-ac07-a6b8ac3c8de3)

#### 4. Instruction Decode with validity
![4](https://github.com/saneeaman9/sanee_riscv/assets/75088597/a051d61a-92a4-4ea6-8317-668d7cdad195)

#### 5. Individual Instruction decode
![5](https://github.com/saneeaman9/sanee_riscv/assets/75088597/db3391a0-db2e-4982-b0ab-b9657da5f804)

#### 6. Register File Read
![6](https://github.com/saneeaman9/sanee_riscv/assets/75088597/e2a64f09-d3e1-4f96-9a38-c2d533b90888)
#### 7. ALU
![7](https://github.com/saneeaman9/sanee_riscv/assets/75088597/3015bf58-58be-4c09-ad07-26a983c2e65f)

#### 8. Register File Write
![8](https://github.com/saneeaman9/sanee_riscv/assets/75088597/0000fd68-55b5-47cd-a067-7f8605cbb64e)

#### 9 Branch Instructions
![9](https://github.com/saneeaman9/sanee_riscv/assets/75088597/2e3b2a42-9844-4f7e-856f-fd050b179c97)

#### 10. Testbench to check functionality
![10](https://github.com/saneeaman9/sanee_riscv/assets/75088597/eba1771d-0e9a-4ffd-a46c-097a656cb0c7)


</details>



<details>
<summary>Day 5 : Complete Pipelined RISC-V Micro Architecture</summary>
<br>



</details>


## OpenLane2 Installation

[Follow this link to install openlane2.](https://github.com/efabless/openlane2)
