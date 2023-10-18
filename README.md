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

![1](https://github.com/saneeaman9/sanee_riscv/assets/75088597/c3abc44c-f728-4c9b-b651-31a69b036da3)


![2](https://github.com/saneeaman9/sanee_riscv/assets/75088597/cb8ca138-0e0b-4ec9-8b7a-32c1889aadd6)


### XOR Gate using Boolean Operator.

![3](https://github.com/saneeaman9/sanee_riscv/assets/75088597/d3c2392e-7ed4-4558-accf-c2a1c77a1d93)


### C) Vectors

![4](https://github.com/saneeaman9/sanee_riscv/assets/75088597/9dfb3d20-6f7e-488b-977a-7eacdd8387ff)


### D) Mux

![5](https://github.com/saneeaman9/sanee_riscv/assets/75088597/fd3fb1d5-55ee-422a-824a-ce2e294a6c82)


### E) Simple Calculator

![6](https://github.com/saneeaman9/sanee_riscv/assets/75088597/c3425895-7d5c-4b32-95f0-6434b8461e58)


### F) Fibonacci Series

![7](https://github.com/saneeaman9/sanee_riscv/assets/75088597/ad5daa80-eb54-409b-ba0e-b43eacf41701)


### G) Up Counter

![8](https://github.com/saneeaman9/sanee_riscv/assets/75088597/6e0cb605-805e-42a4-a640-15786ab01993)


### I) Sequential Calc

![9](https://github.com/saneeaman9/sanee_riscv/assets/75088597/8f9e8eb3-da2c-46bb-97d4-9677312b454f)

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

![10](https://github.com/saneeaman9/sanee_riscv/assets/75088597/7a529342-ffb0-4417-a706-5232e2115e1d)


### J) Pipeline Implementation example.

![11](https://github.com/saneeaman9/sanee_riscv/assets/75088597/7de71cae-d256-4a0c-9c08-13704642d319)


### Validity

> - Easier debugging. 
> - Cleaner design.
> - Better error checking.
> - Automated clock gating.


### K) 2 Cycle Calc with Validity.

![12](https://github.com/saneeaman9/sanee_riscv/assets/75088597/66bfcf3a-8d0c-4f9e-b211-8fd27cdadc72)


### L) Distance Calc.

![13](https://github.com/saneeaman9/sanee_riscv/assets/75088597/12c5e526-9b76-45df-895b-a255fb83f42a)


### Calculator Memory

![14](https://github.com/saneeaman9/sanee_riscv/assets/75088597/0727a9fc-92a2-4049-aad3-78238e8384d2)




</details>


<details>
<summary>Day 4 : Basic RISC-V CPU Micro Architecture</summary>
<br>



</details>



<details>
<summary>Day 5 : Complete Pipelined RISC-V Micro Architecture</summary>
<br>



</details>


## OpenLane2 Installation

[Follow this link to install openlane2.](https://github.com/efabless/openlane2)
