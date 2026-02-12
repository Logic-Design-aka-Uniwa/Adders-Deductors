<p align="center">
  <img src="https://www.especial.gr/wp-content/uploads/2019/03/panepisthmio-dut-attikhs.png" alt="UNIWA" width="150"/>
</p>

<p align="center">
  <strong>UNIVERSITY OF WEST ATTICA</strong><br>
  SCHOOL OF ENGINEERING<br>
  DEPARTMENT OF COMPUTER ENGINEERING AND INFORMATICS
</p>

<hr/>

<p align="center">
  <strong>Logic Design</strong>
</p>

<h1 align="center" style="letter-spacing: 1px;">
  Adders Deductors
</h1>

<p align="center">
  <strong>Vasileios Evangelos Athanasiou</strong><br>
  Student ID: 19390005
</p>

<p align="center">
  <a href="https://github.com/Ath21" target="_blank">GitHub</a> ·
  <a href="https://www.linkedin.com/in/vasilis-athanasiou-7036b53a4/" target="_blank">LinkedIn</a>
</p>

<p align="center">
  Supervisor: Eleni Tsalera, Laboratory Teaching Staff
</p>
<p align="center">
  <a href="https://www.researchgate.net/profile/Eleni-Tsalera-2" target="_blank">UNIWA Profile</a>
</p>

<p align="center">
  Co-supervisor: Georgios Antoniou, Laboratory Teaching Staff
</p>
<p align="center">
  <a href="https://ice.uniwa.gr/en/emd_person/georgios-antoniou/" target="_blank">UNIWA Profile</a>
</p>

<p align="center">
  Athens, April 2021
</p>

---

# Project Overview

This repository contains the documentation and implementation details for **Workshop 2** of the **Digital Design** course at the **University of West Attica**, Department of Informatics and Computer Engineering.

The project focuses on the **theoretical analysis**, **simulation**, and **implementation** of basic arithmetic logic circuits used in digital systems.

---

## Table of Contents

| Section | Folder/File | Description |
|------:|-------------|-------------|
| 1 | `assign/` | Assignment material for the Adders and Deductors workshop |
| 1.1 | `assign/ASSIGNMENT 2.pdf` | Assignment description in English |
| 1.2 | `assign/ΕΡΓΑΣΙΑ 2.pdf` | Assignment description in Greek |
| 2 | `docs/` | Documentation covering adders and deductors theory and implementations |
| 2.1 | `docs/Adders-Deductors.pdf` | English documentation for adders and deductors |
| 2.2 | `docs/Αθροιστές-Αφαιρέτες.pdf` | Greek documentation for adders and deductors |
| 3 | `multisim/` | Multisim circuit simulation files |
| 3.1 | `multisim/semiAdder.ms14` | Half (semi) adder circuit simulation |
| 3.2 | `multisim/fullAdder.ms14` | Full adder circuit simulation |
| 3.3 | `multisim/semiDeductor.ms14` | Half (semi) subtractor circuit simulation |
| 3.4 | `multisim/fullDeductor.ms14` | Full subtractor circuit simulation |
| 3.5 | `multisim/adder4Bits.ms14` | 4-bit adder circuit simulation |
| 4 | `README.md` | Repository overview and usage instructions |

---

## Overview

The workshop covers the design and operation of four fundamental digital circuits used for binary arithmetic:

- **Half Adder**
- **Half Subtractor**
- **Full Adder**
- **Full Subtractor**

For each circuit, the project includes:

- Truth tables  
- Logical equations  
- Multisim simulations  
- Physical implementation descriptions  

---

## Implementation Details

The circuits were designed and simulated using **NI Multisim**.

### Components Used

- **Logic Gates:** AND, OR, NOR, NAND, XOR, XNOR, NOT
- **Hardware Emulation Components:**
  - VCC sources (5V)
  - Ground connections
  - Wires
  - Lamps (2.5V)
  - Switches
- **Measurement Tools:**
  - Oscilloscope for signal analysis

---

## Logic Levels

| Logic State | Voltage Range |
|--------------|--------------|
| Logic **0** | 0V – 0.5V (Ground) |
| Logic **1** | 2.7V – 5V (VCC) |

---

## Circuit Specifications

### 1. Half Adder

The Half Adder calculates the **Sum (S)** and **Carry (C)** of two one-bit binary inputs **X** and **Y**.

#### Logical Equations

- Sum:
  
  $$ 
  S = \overline{X}Y + X\overline{Y} = X \oplus Y 
  $$

- Carry:
  
  $$ 
  C = X \cdot Y 
  $$

#### Truth Table

| X | Y | S (Sum) | C (Carry) |
|---|---|----------|-----------|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 |
| 1 | 1 | 0 | 1 |

---

### 2. Half Subtractor

The Half Subtractor calculates the **Difference (D)** and **Borrow (B)** between two one-bit binary inputs **X** and **Y**.

#### Logical Equations

- Difference:
  
  $$ 
  D = \overline{X}Y + X\overline{Y} = X \oplus Y 
  $$

- Borrow:
  
  $$ 
  B = \overline{X} \cdot Y 
  $$

#### Truth Table

| X | Y | D (Difference) | B (Borrow) |
|---|---|----------------|------------|
| 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 1 |
| 1 | 1 | 0 | 0 |

---

### 3. Full Adder

The Full Adder calculates the sum of three one-bit inputs: **X**, **Y**, and **Carry-in (Cin)**.

Outputs:

- Sum (S)
- Carry-out (Cout)

Logical equations:

$$
S = X \oplus Y \oplus Cin 
$$

$$
Cout = XY + Cin(X \oplus Y) 
$$

---

### 4. Full Subtractor

The Full Subtractor performs subtraction including a **Borrow-in (Bin)** input.

Outputs:

- Difference (D)
- Borrow-out (Bout)

Logical equations:

$$
D = X \oplus Y \oplus Bin 
$$
$$
Bout = \overline{X}Y + Bin(\overline{X} \oplus Y) 
$$

---

## Conclusion

This workshop demonstrates the construction and operation of basic arithmetic circuits forming the foundation of **Arithmetic Logic Units (ALUs)** in modern processors. The simulations and implementations help reinforce understanding of binary arithmetic and digital circuit behavior.

---

# Installation & Setup Guide

This repository contains laboratory simulations and analysis for **Circuit Theory**, focusing on **RLC series and parallel circuits** and their resonance behavior.  

All simulations are implemented in **NI Multisim**.

---

## Prerequisites

### Required Software
- **NI Multisim 14** (or later)  
  Ensure your system meets the requirements for running `.ms14` files.  
  Download from [NI Multisim](https://www.ni.com/en-us/shop/electronic-test-instrumentation/application-software-for-electronic-test-and-instrumentation-category/what-is-multisim.html).

### Optional Software
- **PDF Viewer** for documentation: `Coordination.pdf` / `Συντονισμός.pdf`

---

## Installation Steps

### 1. Clone the Repository
```bash
git clone https://github.com/Circuit-Theory/Coordination.git
```

### 2. Navigate to Project Directory
```bash
cd Coordination
```
Ensure the following folder structure exists:
```bash
assign/
docs/
multisim/
```

---

## Multisim Simulation Files

The repository includes two key simulation files:

| File  | Description |
|------:|-------------|
| multisim/CoordinationSerial.ms14 |  RLC series circuit simulation |
| multisim/CoordinationParallel.ms14 |  RLC parallel circuit simulation |


### 3. Open a Simulation in Multisim
- Launch NI Multisim.
- Select File → Open.
- Navigate to the `multisim/` folder.
- Open the desired `.ms14` file (series or parallel circuit).
- Wait for the circuit topology to load.

---

## Open the Documentation
1. Navigate to the `docs/` directory
2. Open the report corresponding to your preferred language:
    - English: `Coordination.pdf`
    - Greek: `Συντονισμός.pdf`
