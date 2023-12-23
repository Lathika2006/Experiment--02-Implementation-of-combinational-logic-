# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime

## Theory

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

NAND gate is actually a combination of two logic gates i.e. AND gate followed by NOT gate. So its output is complement of the output of an AND gate.This gate can have minimum two inputs, output is always one. By using only NAND gates, we can realize all logic functions: AND, OR, NOT, X-OR, X-NOR, NOR. So this gate is also called as universal gate. First note that the entire expression is inverted and we have three terms ANDed. This means that we must use a 3-input NAND gate. Each of the three terms is, itself, a NAND expression. Finally, negated single terms can be generates with a 2-input NAND gate acting as an inverted.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')'

## Logic Diagram

Using NOR gates NOR gate is actually a combination of two logic gates: OR gate followed by NOT gate. So its output is complement of the output of an OR gate. This gate can have minimum two inputs, output is always one. By using only NOR gates, we can realize all logic functions: AND, OR, NOT, Ex-OR, Ex-NOR, NAND. So this gate is also called universal gate. Designing a circuit with NOR gates only uses the same basic techniques as designing a circuit with NAND gates; that is, the application of deMorgan’s theorem. The only difference between NOR gate design and NAND gate design is that the former must eliminate product terms and the later must eliminate sum terms.

F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'

## Procedure

1.Create a project with required entities.
2.Create a module along with respective file name.
3.Run the respective programs for the given boolean equations.
4.Run the module and get the respective RTL outputs.
5.Create university program(VWF) for getting timing diagram.
6.Give the respective inputs for timing diagram and obtain the results.

## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: LATHIKA L.J
RegisterNumber: 23012411 

*/

##OUTPUT:

## Code:

![image](https://github.com/Lathika2006/Experiment--02-Implementation-of-combinational-logic-/assets/148959215/1d63bd22-a346-4bf8-9e47-d5a6726d4387)

## Truth table:

![image](https://github.com/Lathika2006/Experiment--02-Implementation-of-combinational-logic-/assets/148959215/d3c49bd1-68e5-464b-b0f0-4c3d1fcf3d79)

## RTL Diagram:

![image](https://github.com/Lathika2006/Experiment--02-Implementation-of-combinational-logic-/assets/148959215/13a304d7-7036-4067-a3ad-05a98c4c8e3e)

## Timing Diagram:

![image](https://github.com/Lathika2006/Experiment--02-Implementation-of-combinational-logic-/assets/148959215/08c3edfd-0245-4d9f-a5e6-88c32b89f029)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
