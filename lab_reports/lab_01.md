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
