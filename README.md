# Experiment--04-Implementation-of-combinational-logic-using-universal-gates
Implementation of combinational logic using universal-gates
 
## AIM:
To implement the given logic function using NAND and NOR gates and to verify its operation in Quartus using Verilog programming.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')' using NAND gate
F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')' using NOR gate
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. 

## Using NAND gates
NAND gate is actually a combination of two logic gates i.e. AND gate followed by NOT gate. So its output is complement of the output of an AND gate.This gate can have minimum two inputs, output is always one. By using only NAND gates, we can realize all logic functions: AND, OR, NOT, X-OR, X-NOR, NOR. So this gate is also called as universal gate. First note that the entire expression is inverted and we have three terms ANDed. This means that we must use a 3-input NAND gate. Each of the three terms is, itself, a NAND expression. Finally, negated single terms can be generates with a 2-input NAND gate acting as an inverted.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')'

## Logic Diagram

Using NOR gates
NOR gate is actually a combination of two logic gates: OR gate followed by NOT gate. So its output is complement of the output of an OR gate. This gate can have minimum two inputs, output is always one. By using only NOR gates, we can realize all logic functions: AND, OR, NOT, Ex-OR, Ex-NOR, NAND. So this gate is also called universal gate. Designing a circuit with NOR gates only uses the same basic techniques as designing a circuit with NAND gates; that is, the application of deMorgan’s theorem. The only difference between NOR gate design and NAND gate design is that the former must eliminate product terms and the later must eliminate sum terms.

F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'

## Logic Diagram
## Procedure
## Program:
/*
Program to implement the given logic function using NAND and NOR gates and to verify its operations in quartus using Verilog programming.
Developed by:lingeswaran k
RegisterNumber:22005148
*/
## RTL realization

## Output:
NAND
## RTL
![image](https://user-images.githubusercontent.com/119103865/213094591-e5db02b5-8f70-4ad8-94f7-4e90d80c338f.png)

## Timing Diagram
![image](https://user-images.githubusercontent.com/119103865/213094618-e240f4e9-cd51-4b3b-8a6c-14c6f210422d.png)

## Truth table
![image](https://user-images.githubusercontent.com/119103865/213094778-1315b5b9-7769-4abe-b7a5-9bbf8d76d2ab.png)

NOR
RTL
![image](https://user-images.githubusercontent.com/119103865/213094866-088a0d90-7745-4320-b6f0-92de9f9c663a.png)
Timing diagram
![image](https://user-images.githubusercontent.com/119103865/213094936-5019b34d-af59-4a8a-9ba2-e60b1162d268.png)
Truth table
![image](https://user-images.githubusercontent.com/119103865/213094972-30d485e7-f15a-45a4-90d0-e242e8a284fc.png)

## Result:
Thus the given logic functions are implemented using NAND and NOR gates and their operations are verified using Verilog programming.
