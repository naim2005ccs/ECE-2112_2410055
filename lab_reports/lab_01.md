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

<img width="858" height="211" alt="image" src="https://github.com/user-attachments/assets/6ec8463e-b050-4acc-bf3d-59f54b89a4b6" />
<img width="892" height="297" alt="image" src="https://github.com/user-attachments/assets/5b782784-0f03-4a7c-a841-dcd0d29a5946" />



A ----\
       NAND ---- Output
A ----/

---

### AND Gate Using NAND

<img width="1339" height="315" alt="image" src="https://github.com/user-attachments/assets/0f2ba924-d3b5-44d1-b91b-0450cdc2dc96" />
<img width="1346" height="340" alt="image" src="https://github.com/user-attachments/assets/4813df9f-897d-4221-b91a-3d8ea86e9dd1" />



A ----\
       NAND ----\
B ----/          \
                  NAND ---- Output
               ___/

---

### OR Gate Using NAND

<img width="1363" height="545" alt="image" src="https://github.com/user-attachments/assets/b59f3b92-7c20-4f10-908a-1ca65eb2c799" />
<img width="1368" height="507" alt="image" src="https://github.com/user-attachments/assets/4d07368d-eaea-47b3-ab49-94acd3b5a630" />



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

<img width="866" height="248" alt="image" src="https://github.com/user-attachments/assets/25258b42-15b3-4352-aeb3-5211aee3d7a0" />
<img width="952" height="282" alt="image" src="https://github.com/user-attachments/assets/192a2268-c627-41e2-9858-5fdd71c11378" />



A ----\
       NOR ---- Output
A ----/

---

### OR Gate Using NOR

<img width="1374" height="373" alt="image" src="https://github.com/user-attachments/assets/ef65f1dc-f6e4-4483-9181-e8c7b8d890c9" />
<img width="1373" height="328" alt="image" src="https://github.com/user-attachments/assets/cae25496-0524-4a9c-9d52-feec3bff20c8" />



A ----\
       NOR ----\
B ----/         \
                 NOR ---- Output

---

### AND Gate Using NOR

<img width="1333" height="550" alt="image" src="https://github.com/user-attachments/assets/d3240ac6-2e5d-4cff-bacd-3d52f1be3b8d" />
<img width="1322" height="554" alt="image" src="https://github.com/user-attachments/assets/e9dec8b3-48f2-42d8-b370-5f0b78df1c19" />



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

<img width="1307" height="558" alt="image" src="https://github.com/user-attachments/assets/84fc7392-846c-40d6-a708-3e7c356e3e51" />


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

<img width="884" height="497" alt="image" src="https://github.com/user-attachments/assets/5502db73-85ae-472c-8e5b-6ede33b90feb" />


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
