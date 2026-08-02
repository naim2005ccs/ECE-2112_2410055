# Digital Logic Design Laboratory Report

## Table of Contents

1. Introduction
2. Objectives
3. Software Used
4. Experiment 1: Implementation of AND, OR, and NOT Gates Using NAND Gate
5. Experiment 2: Implementation of AND, OR, and NOT Gates Using NOR Gate
6. Experiment 3: Binary to BCD Converter
7. Experiment 4: Single Bit Full Adder
8. Conclusion

---

# Introduction

Digital systems are built using various logic gates and combinational circuits. Universal gates such as NAND and NOR can be used to implement all other basic logic gates. In this laboratory experiment, NAND and NOR gates were used to design AND, OR, and NOT gates. A Binary to BCD Converter and a Single Bit Full Adder were also implemented and verified using Logisim Evolution.

---

# Objectives

- To understand the concept of universal gates.
- To implement AND, OR, and NOT gates using NAND gates.
- To implement AND, OR, and NOT gates using NOR gates.
- To design and verify a Binary to BCD Converter.
- To design and verify a Single Bit Full Adder.
- To simulate digital circuits using Logisim Evolution.

---

# Software Used

- Logisim Evolution

---

# Experiment 1

# Implementation of AND, OR, and NOT Gates Using NAND Gate

## Theory

The NAND gate is known as a Universal Gate because any digital logic circuit can be implemented using only NAND gates.

---

## Circuit Diagram

### NOT Gate Using NAND

<img width="544" height="182" alt="image" src="https://github.com/user-attachments/assets/79a411e3-781d-4457-b487-1150d6d1a7ba" />



A ----\
       NAND ---- Output
A ----/

---

### AND Gate Using NAND

<img width="882" height="299" alt="image" src="https://github.com/user-attachments/assets/4c46c054-c498-433f-a911-61a74a0c3bf3" />



A ----\
       NAND ----\
B ----/          \
                  NAND ---- Output
               ___/

---

### OR Gate Using NAND

<img width="901" height="358" alt="image" src="https://github.com/user-attachments/assets/43fcf4a7-7da4-40f4-8e2d-b083a77185f2" />



A ----\
       NAND ----\
A ----/          \
                  NAND ---- Output
               ___/
B ----\
       NAND ----/
B ----/

---

## Truth Table

### NOT Gate

| Input (A) | Output (Y) |
|-----------|------------|
| 0 | 1 |
| 1 | 0 |

---

### AND Gate

| A | B | Y |
|---|---|---|
|0|0|0|
|0|1|0|
|1|0|0|
|1|1|1|

---

### OR Gate

| A | B | Y |
|---|---|---|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|1|

---

## Observation

The outputs obtained from the simulation matched the theoretical truth tables. This verifies that NAND gates can successfully implement all basic logic gates.

---

# Experiment 2

# Implementation of AND, OR, and NOT Gates Using NOR Gate

## Theory

The NOR gate is also a Universal Gate. Every basic logic gate can be implemented using only NOR gates.

---

## Circuit Diagram

### NOT Gate Using NOR

<img width="567" height="184" alt="image" src="https://github.com/user-attachments/assets/e73ef4ed-2387-476e-b6ba-8c8dc5fb847d" />



A ----\
       NOR ---- Output
A ----/

---

### OR Gate Using NOR

<img width="1074" height="319" alt="image" src="https://github.com/user-attachments/assets/225228d0-8da5-44c9-b91d-95fce08138c0" />



A ----\
       NOR ----\
B ----/         \
                 NOR ---- Output

---

### AND Gate Using NOR

<img width="1045" height="393" alt="image" src="https://github.com/user-attachments/assets/f3769afa-2243-4931-b42a-e838cdcb0e98" />


A ----\
       NOR ----\
A ----/         \
                 NOR ----\
                           NOR ---- Output
B ----\         /
       NOR ----/
B ----/

---

## Truth Table

### NOT Gate

| Input (A) | Output (Y) |
|-----------|------------|
|0|1|
|1|0|

---

### AND Gate

|A|B|Y|
|---|---|---|
|0|0|0|
|0|1|0|
|1|0|0|
|1|1|1|

---

### OR Gate

|A|B|Y|
|---|---|---|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|1|

---

## Observation

The outputs obtained matched the expected truth tables, confirming that NOR is also a universal gate.

---

# Experiment 3

# Binary to BCD Converter

## Theory

A Binary to BCD Converter converts a binary number into its corresponding Binary Coded Decimal (BCD) representation. Each decimal digit is represented by four binary bits.

---

## Circuit Diagram

<img width="900" height="328" alt="image" src="https://github.com/user-attachments/assets/4eecfedd-6b57-46e7-ac36-bdee89082dda" />



---

## Sample Input-Output Table

| Binary | Decimal | BCD |
|---------|----------|------|
|0000|0|0000|
|0001|1|0001|
|0010|2|0010|
|0011|3|0011|
|0100|4|0100|
|0101|5|0101|
|0110|6|0110|
|0111|7|0111|
|1000|8|1000|
|1001|9|1001|

---

## Working Principle

The converter receives a binary input and generates its equivalent BCD output. For binary values from 0 to 9, the BCD output is identical to the binary representation of the decimal digit.

---

## Observation

The converter correctly produced the BCD representation for all tested binary inputs.

---

# Experiment 4

# Single Bit Full Adder

## Theory

A Full Adder is a combinational circuit that adds three one-bit binary inputs:

- A
- B
- Carry In (Cin)

It produces two outputs:

- Sum
- Carry Out (Cout)

---

## Boolean Expressions

Sum

Sum = A ⊕ B ⊕ Cin

Carry

Cout = (A · B) + (Cin · (A ⊕ B))

---

## Circuit Diagram


<img width="498" height="333" alt="image" src="https://github.com/user-attachments/assets/11ba1817-6f80-4b8c-b096-1e59ee995833" />


---

## Truth Table

|A|B|Cin|Sum|Cout|
|---|---|---|---|---|
|0|0|0|0|0|
|0|0|1|1|0|
|0|1|0|1|0|
|0|1|1|0|1|
|1|0|0|1|0|
|1|0|1|0|1|
|1|1|0|0|1|
|1|1|1|1|1|

---

## Working Principle

The Full Adder first calculates the Sum by performing XOR operations on the three inputs. The Carry Out is generated whenever two or more inputs are HIGH. The circuit is widely used in binary arithmetic operations and serves as the building block for multi-bit adders.

---

## Observation

The simulated outputs matched the theoretical truth table for all possible input combinations.

---

# Conclusion

In this laboratory experiment, the implementation of basic logic gates using universal gates was successfully verified. NAND and NOR gates were used to construct AND, OR, and NOT gates, demonstrating their universality. A Binary to BCD Converter and a Single Bit Full Adder were also designed and simulated successfully using Logisim Evolution.

The simulation results matched the theoretical truth tables, confirming the correctness of each circuit. This experiment provided a practical understanding of combinational logic design and the implementation of digital circuits using logic gates.

---

# References

1. M. Morris Mano, *Digital Design*, Pearson Education.
2. Thomas L. Floyd, *Digital Fundamentals*.
3. Logisim Evolution Documentation.
4. 
